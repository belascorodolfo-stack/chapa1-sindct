# Site da Chapa 1 · como publicar e onde ficam as sugestões

**No ar:** https://chapa1-sindct.onrender.com (Render, plano gratuito, publicado em 26/10/2026).
Planilha das sugestões: "Sugestões Chapa 1 - SindCT 2026 (respostas)" no Google Drive do Rodolfo.
Carta com o QR novo: `Downloads\Chapa1_carta_FRENTE_E_VERSO_QR_novo.pdf`.

Página: `index.html` (programa da Chapa 1, Eleições SindCT 2026, com sugestão por eixo, anônima ou
identificada). Site separado do CAESPRO Gestão. As sugestões vão para uma planilha Google do Rodolfo.

## 1. Formulário Google (onde as sugestões ficam guardadas)

Na conta Google do Rodolfo, em forms.google.com → **Formulário em branco**:

1. Título: `Sugestões · Chapa 1`.
2. Crie 7 perguntas, todas do tipo **Resposta curta**, exceto a 2 (**Parágrafo**), nesta ordem e sem
   marcar "obrigatória":
   1. `Eixo`
   2. `Sugestão` (Parágrafo)
   3. `Identificação`
   4. `Nome completo`
   5. `Telefone`
   6. `E-mail`
   7. `Local de trabalho`
3. Engrenagem **Configurações** → **Respostas**: deixe **desligado** "Coletar endereços de e-mail" e
   "Limitar a 1 resposta" (senão o formulário exige login do Google e o envio da página falha).
4. Aba **Respostas** → ícone verde **Vincular ao Planilhas** → Criar planilha. É nela que você lê tudo.
5. Menu **⋮** (três pontinhos) → **Obter link preenchido** → escreva qualquer coisa em cada pergunta
   (ex.: `a`, `b`, `c`…) → **Obter link** → **Copiar link** e mande esse link para o Claude.
   Dele saem o endereço do formulário e os códigos `entry.NNNN` de cada pergunta, que vão para a
   configuração `ENVIO` no começo do script da página.

## 2. Endereço na internet (provedor Render, mesmo do CAESPRO Gestão)

1. No GitHub (conta `belascorodolfo-stack`), crie um repositório **vazio** chamado `chapa1-sindct`
   (sem README). Pode ser privado. O Claude envia os arquivos desta pasta para ele.
2. No Render (dashboard.render.com) → **New** → **Static Site** → escolha o repositório
   `chapa1-sindct` → Name: `chapa1-sindct` → Build Command: em branco → Publish Directory: `.` →
   **Create Static Site**. O endereço fica `https://chapa1-sindct.onrender.com` (se o nome estiver
   livre; senão o Render sugere outro). Site estático no Render é gratuito.
3. O site foi ligado pelo endereço público do repositório, então **não atualiza sozinho**: depois de
   cada `git push`, no Render abra `chapa1-sindct` → **Manual Deploy** → **Deploy latest commit**.
4. Fotos dos integrantes (27/10/2026): recortadas das originais em `Meu Drive\Sindicatootos`
   (a da Silvia continua a antiga). Ficam embutidas no `index.html`.

## 3. QR Code da carta

Com o endereço definitivo, o Claude gera o QR Code e troca o da carta
(`Chapa1_carta_FRENTE_E_VERSO.pdf`, frente, quadro "Programa completo e sua sugestão em cada eixo")
no mesmo lugar e tamanho. Só imprimir depois de testar: apontar a câmera, abrir a página, mandar
uma sugestão de teste e ver a linha chegar na planilha.

## Dados pessoais (LGPD)

A página avisa, quando a pessoa escolhe se identificar: "Seus dados ficam só com a Chapa 1, são
usados apenas para responder à sua sugestão e não são repassados a ninguém." Só o Rodolfo tem acesso
à planilha. Depois da eleição, apagar os dados de contato que não forem mais necessários.
