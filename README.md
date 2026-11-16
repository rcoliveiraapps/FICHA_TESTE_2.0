# Ficha de Vistoria - Itazi Engenharia v17

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

Cache offline: `ficha-17`.
