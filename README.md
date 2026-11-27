# SimulaCard IA

Simulador de treinamento para atendentes de operações de **cartão alimentação e refeição**.
O operador conversa (por texto ou voz) com um cliente virtual — usuário, gestor (empresa ou órgão público) ou lojista — e recebe uma avaliação detalhada ao final.

> Todos os dados (nomes, CPFs, CNPJs, cartões, empresas e órgãos) são **fictícios**.

## Como usar
Abra o endereço publicado pelo GitHub Pages (veja abaixo). Não precisa instalar nada.

## Publicar no GitHub Pages
1. Crie um repositório no GitHub (público) e envie estes dois arquivos: `index.html` e `README.md`.
   - Pelo site: **Add file → Upload files**, arraste os arquivos e clique em **Commit changes**.
2. Vá em **Settings → Pages**.
3. Em **Build and deployment**, escolha **Deploy from a branch**, branch **main** e pasta **/ (root)**. Salve.
4. Em cerca de 1 minuto o endereço aparece no topo da página: `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

Pelo terminal:
```bash
git init
git add .
git commit -m "SimulaCard IA"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
git push -u origin main
```

## Configurar a IA e a voz (dentro do app)
Em **Administração → Configurações**:
- **Chave da Anthropic (Claude):** ativa o cliente com IA real e a avaliação por IA.
- **Chave da ElevenLabs:** ativa vozes de IA (opcional).
- **Testar microfone:** confirma o microfone e o reconhecimento de voz no seu aparelho.

As chaves ficam só na memória do navegador e precisam ser digitadas de novo ao recarregar a página.
**Nunca coloque chaves dentro do `index.html` nem no repositório:** o repositório é público.

## Observações
- Microfone e reconhecimento de voz funcionam no **Google Chrome e no Microsoft Edge**, com internet.
- Sem chave da Anthropic, o app usa frases prontas e uma avaliação básica por regras.
- Para atualizar, troque o `index.html` no repositório e faça um novo commit.
