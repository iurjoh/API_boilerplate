# JSHint API front end

[English](README.md)

## Ideia e processo

Cliente estático de estudo para API JSHint, não boilerplate de backend. Código revisado em 01/10/2026. Não foram encontrados planejamento datado ou wireframes nos arquivos revisados. Interface recebe nome de arquivo, URL ou JavaScript, opções e mostra status/resultados em modal.

## Arquitetura e design

`index.html` carrega Bootstrap 5.0.0-beta2, Font Awesome, CSS local e `assets/js/script.js`. Script cria modal, coleta FormData, junta opções e usa fetch para URL histórica Heroku. Envia chave no header Authorization do POST e query do status. Exibe resultados por strings HTML. Não há implementação de servidor na raiz revisada.

## Preview local

```bash
python3 -m http.server 8000
```

Abra `http://localhost:8000/`. Sugestão de preview, não execução verificada. Não clique Check Key ou Run Checks com chave versionada ou código privado. Controles fazem requisições externas; abrir exemplo não comprova disponibilidade, permissão ou tratamento seguro de dados.

## Testes, privacidade e limites

Suíte não encontrada na listagem revisada. Nenhuma requisição, validação de chave ou teste executado; disponibilidade atual da API desconhecida.

Cliente público contém API_KEY literal não vazia. Valor não repetido aqui; validade atual desconhecida. Código do navegador não mantém segredo de serviço privado. Revise revogação e desenho de credenciais separadamente antes de uso real.

Cliente envia código/URLs a endpoint de terceiro e insere strings da resposta em innerHTML. Revise consentimento de envio, entradas/saídas, erros de rede/JSON e renderização segura. Teste opções, entrada vazia e modal só com dados fictícios e serviço de teste autorizado. `displayException` também atribui results sem declaração local.

## Capturas

Nenhuma captura verificada ou adicionada. Capturas futuras em `docs/assets/` devem usar código fictício e remover chaves, URLs sensíveis e resultados privados. Identifique como cliente demonstrativo, não serviço funcional sem verificação segura do endpoint.

## Créditos e licença

Material de template/curso do Code Institute e dependências mantêm direitos originais, sem licença nova. README original preservado no [apêndice em inglês](README.md#original-readme), como referência histórica.
