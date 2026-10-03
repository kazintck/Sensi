# FF Sense Lab

Site completo de demonstração para consulta de UID e geração de sensibilidade.

## Como ativar a consulta real do jogador

1. Crie uma conta/projeto no provedor da API escolhido e obtenha sua API Key.
2. Copie `.env.example` para `.env`.
3. Coloque sua chave em `FF_API_KEY`.
4. Instale Node.js 18+.
5. Execute:

```bash
npm install
npm start
```

6. Abra `http://localhost:3000`.

## Importante

A chave fica no backend e não no navegador. O endpoint `/api/player` faz a ponte com a API externa.

A integração foi preparada para o endpoint documentado como `/api/v1/info`, com `uid`, `region` e header `x-api-key`. APIs de terceiros podem alterar endereço, autenticação ou formato de resposta; se isso ocorrer, ajuste `FF_API_BASE` ou a normalização em `server.js`.

O gerador de sensibilidade é uma fórmula de demonstração e não altera configurações dentro do Free Fire. O Access criado pelo site é um código interno da aplicação.
