# Mulheres em Ação | Outubro Rosa 🌸🎀
**Volkswagen PU Taubaté**

Web App Mobile-First desenvolvida para a campanha do **Outubro Rosa - Mulheres em Ação (Volkswagen PU Taubaté)**, permitindo que os participantes capturem fotos ou escolham da galeria, apliquem molduras temáticas personalizadas em alta definição (1080x1920) e compartilhem nas redes sociais (Instagram Stories, WhatsApp) ou façam download direto.

---

## ✨ Funcionalidades

- 📱 **Mobile-First & PWA Ready:** Projetada especificamente para acesso rápido via leitura de **QR Code** no smartphone durante eventos e ações presenciais.
- 📐 **Moldura Adaptável e Ajustável:** O visor se adapta dinamicamente a qualquer modelo e proporção de tela de smartphone (iPhones, telas compridas 20:9, etc.), com botão de alternância entre "Moldura 9:16" e "Tela Cheia".
- 🔍 **Controle Interativo de Zoom & Reposicionamento:** Permite dar zoom na foto e arrastar com o dedo na tela para encaixar o rosto com perfeição dentro do espaço vazado da moldura.
- 📸 **Câmera Integrada ao Vivo:** Permite captura instantânea com alternância entre câmera frontal (selfie) e câmera traseira.
- 🖼️ **3 Molduras Exclusivas (1080x1920):** Troca dinâmica e em tempo real sobre o visor da câmera.
- 📁 **Suporte a Galeria:** Opção de selecionar foto da galeria do aparelho caso prefira ou caso a câmera esteja indisponível.
- 🎨 **Processamento em Alta Resolução:** Canvas 1080x1920 que une a foto e a moldura respeitando os ajustes de zoom e deslocamento aplicados pelo usuário.
- 🎀 **Identidade Visual Oficial Outubro Rosa:** Logo comemorativa com o laço rosa sobreposto e favicons para navegador e tela de início.
- 📲 **Compartilhamento Nativo & Download:** Integração com o menu de compartilhamento do smartphone (`Web Share API`) e download direto em PNG.

---

## 📁 Estrutura de Arquivos

```text
camera-outubro-rosa/
├── index.html            # Aplicação completa (HTML5, CSS3 Glassmorphism, JS Vanilla)
├── logo.png              # Emblema comemorativo com o laço rosa sobreposto
├── logo.jpg              # Imagem original de apoio
├── laco_rosa.png         # Laço rosa oficial da campanha (PNG transparente)
├── favicon.ico           # Favicon do site em múltiplos tamanhos
├── favicon-32x32.png     # Ícone para navegadores
├── apple-touch-icon.png  # Ícone para atalho no celular
├── moldura1.png          # Moldura 1 (1080x1920 PNG transparente)
├── moldura2.png          # Moldura 2 (1080x1920 PNG transparente)
├── moldura3.png          # Moldura 3 (1080x1920 PNG transparente)
└── README.md             # Documentação e instruções de deploy
```

---

## 🚀 Como Hospedar (Deploy na Vercel)

Esta é uma aplicação estática (Pure HTML/JS/CSS), o que significa que o deploy é instantâneo e gratuito na [Vercel](https://vercel.com):

1. Acesse o seu dashboard na **Vercel**.
2. Clique em **"Add New..."** > **"Project"**.
3. Importe o repositório `pri-pereira/mulheres-em-acao-outubro-rosa`.
4. Mantenha as configurações padrão (Framework Preset: **Other** / Root Directory: `./`).
5. Clique em **"Deploy"**.
6. Pronto! Você receberá uma URL pública com HTTPS (essencial para o funcionamento da câmera no celular) e poderá gerar o **QR Code** para a campanha.

---

## 💻 Teste Local

Para testar localmente em seu computador:

```bash
# Com Python:
python -m http.server 3000

# Ou com Node:
npx serve .
```

Abra no navegador: `http://localhost:3000` (lembre-se de que a API de câmera `getUserMedia` requer `localhost` ou `https://` para funcionar).
