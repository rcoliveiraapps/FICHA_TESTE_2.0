# Ficha de Vistoria - Itazi Engenharia v18

Versão consolidada para uso em campo.

## Alterações principais
- Ícones **? Ajuda rápida** e **⚙ Configurações** no topo do app. Configurações saiu do rodapé.
- Pasta escolhida em Configurações passa a ser usada de fato pelo download, com estrutura Ano / Mês / Projeto. A referência da pasta é guardada no IndexedDB quando suportado. Downloads é usado como fallback quando não há autorização.
- Croqui preserva o motor geométrico existente, ganha instrução passo a passo e comando Ajustar à tela.
- **Nº da Vistoria** separado da **Referência Cadastral**. O Nº é operacional e sequencial por projeto; Referência Cadastral identifica o imóvel e é opcional.
- Consulta de histórico pela Referência Cadastral, com opção de copiar endereço/localização anterior.
- **Concluir vistoria** abre conferência de essenciais e atenções e registra data/hora e vistoriador.
- Ajuda rápida integrada para início, localização, fotos, croqui, conclusão e downloads.
- Mantidas as diferenças originais entre Urbana e Rural.

Cache offline: `ficha-18`.


## Correção v18
A seleção da pasta agora executa uma gravação de teste. Navegadores que fornecem um diretório gravável sem os métodos `queryPermission/requestPermission` também são aceitos. Se a gravação falhar, o app informa claramente antes de usar Downloads.

## Correção v19
Corrigido um erro de escopo no módulo v17/v18: as funções de pasta e de conclusão usavam auxiliares (`F`, `vv`, `esc`) definidos dentro de outro módulo JavaScript e, por isso, não estavam acessíveis em tempo de execução. Isso explicava simultaneamente o salvamento cair em Downloads e o botão Concluir Vistoria aparentar não mudar. Os auxiliares agora são locais ao módulo e acessíveis por todas essas funções.

## Alteração v20
A estrutura automática das pastas passa a priorizar o projeto: `Projeto / Ano / Mês`. O texto em Configurações e na Ajuda rápida foi ajustado para o mesmo padrão. Se o projeto estiver vazio, usa `SEM-PROJETO / Ano / Mês`.
