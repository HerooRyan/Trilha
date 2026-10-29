# Ativação da correção dissertativa com Google Search

O serviço do Worker (`ai-worker.js`) usa a variável secreta `GEMINI_API_KEY`. Crie a chave na sua própria conta do Google AI Studio e guarde-a como um **Secret** no Worker `trilha-ai` do Cloudflare. Não coloque a chave em `index.html`, no GitHub ou nesta conversa.

No Cloudflare, abra o Worker `trilha-ai` → **Settings** → **Variables and Secrets** → **Add** → **Secret**. Use o nome `GEMINI_API_KEY` e salve. Em seguida, publique a versão atualizada de `ai-worker.js` no Worker para ativar as rotas de perguntas e de correção.

O Google informa que o nível gratuito do Gemini API inclui até 500 solicitações diárias de pesquisa grounding com Google Search, sujeito aos limites vigentes da conta. Não habilite cobrança se quiser manter o uso sem custo; as cotas podem limitar temporariamente as correções.