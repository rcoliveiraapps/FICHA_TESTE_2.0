# Ficha de Vistoria - Itazi Engenharia

Aplicativo web progressivo (PWA) para fichas de vistoria urbana e rural.

## Publicar no GitHub Pages
1. Extraia este pacote na raiz do repositório.
2. Faça commit e push para a branch `main`.
3. Em **Settings > Pages**, selecione **Deploy from a branch**, branch `main`, pasta `/ (root)`.
4. Abra a URL publicada uma vez com internet para o cache offline ser criado.

## Melhorias incluídas
- múltiplos telefones e interessados adicionais;
- número e complemento do imóvel separados;
- e-mail disponível na ficha rural;
- localização de cadastro por Referência Cadastral;
- exibição de latitude/longitude e UTM/SIRGAS 2000;
- edição posterior das coordenadas das fotos;
- exportação/importação individual em JSON;
- seleção de formatos para baixar ou compartilhar;
- cópia opcional em pasta escolhida pelo usuário quando o navegador oferece File System Access;
- nomenclatura padronizada de arquivos;
- CSV UTF-8 com BOM e separador ponto e vírgula;
- cache offline atualizado para `ficha-11`, incluindo o ícone maskable e `enhancements.js`.

## Observação de compatibilidade
A escolha automática de pasta depende do navegador. Em navegadores sem `showDirectoryPicker`, os arquivos são enviados para a pasta padrão de Downloads.
