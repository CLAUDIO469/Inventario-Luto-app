
# Inventário de Luto Prolongado — Expo app (com export e partilha)

Este é um projecto inicial em **Expo (React Native)** pronto para rodar no seu computador e testar no telemóvel com o Expo Go.

## O que foi implementado
- Tela Splash / Capa, Home, Questionário e Resultados.
- Semáforo de interpretação com os pontos de corte 30 (atenção) e 35 (alto risco).
- Salvamento no dispositivo via AsyncStorage.
- Exportar resultado para **PDF** (expo-print) e **CSV** (expo-file-system) e partilhar (expo-sharing).
- Interface simples com botões e inputs — ideal para testes e evolução.

## Pré-requisitos (passo a passo para leigos)
1. Instale o **Node.js** (versão LTS) — https://nodejs.org/
2. Instale o **Expo CLI** globalmente:
   ```bash
   npm install -g expo-cli
   ```
3. Descompacte o ZIP do projecto e abra a pasta no terminal.
4. Instale dependências:
   ```bash
   npm install
   ```
5. Inicie o servidor de desenvolvimento:
   ```bash
   npm start
   ```
6. No seu telemóvel, instale o app **Expo Go** (Android: Play Store, iOS: App Store) e use o leitor de QR mostrado no terminal/na página web do Expo para abrir o app no telemóvel.

## Publicar como site (PWA) — opção totalmente gratuita
- Pode publicar a versão web do app e distribuir como PWA (instalável no telemóvel) sem pagar taxas nas lojas.
- Opções gratuitas populares:
  - Vercel (https://vercel.com) — integra com GitHub e faz deploy automático.
  - Netlify (https://netlify.com) — também suporta deploy automático por Git.
- Guia rápido:
  1. Faça build web: `expo build:web` ou `npm run web` conforme as instruções do Expo.
  2. Conecte repositório no Vercel/Netlify e selecione o diretório `web-build` ou `web` conforme configuração.
- (Referência: docs Expo sobre publicar websites e Vercel/Netlify). 

## Publicar em lojas (opções pagas obrigatórias)
- **Google Play:** requer conta de desenvolvedor (taxa única US$25). Veja: https://support.google.com/googleplay/android-developer/answer/6112435.  
- **Apple App Store:** requer Apple Developer Program (US$99/ano). Veja: https://developer.apple.com/support/compare-memberships/
- Com Expo, pode usar **EAS Build** para criar binários para enviar às lojas. (Expo EAS docs).

## Sugestões de fluxo para um iniciante (passo a passo)
1. Teste no seu telemóvel usando Expo Go (rápido e grátis).  
2. Ajuste textos e cores no código (em `screens/`).  
3. Publique a versão web como PWA no Vercel — assim qualquer pessoa pode usar via browser sem instalar nada.  
4. Se, no futuro, quiser publicar nas lojas, abra conta no Google Play (US$25) e/ou Apple (US$99/ano) e siga a documentação do Expo EAS Build.

## Recursos e documentação útil
- Expo docs (começar): https://expo.dev/.  
- Expo Print: https://docs.expo.dev/versions/latest/sdk/print/.  
- Expo Sharing: https://docs.expo.dev/versions/latest/sdk/sharing/.  
- EAS Build: https://docs.expo.dev/build/introduction/.  
- Vercel: https://vercel.com.  
- Netlify: https://netlify.com.  

---

Se quiser, eu posso:
- Gerar outro ZIP final com versões otimizadas (ícones, screenshots) — já posso incluir.  
- Fazer o deploy web para Vercel/Netlify para si (vou descrever passo-a-passo com prints e comandos).  
- Preparar instruções detalhadas para abrir contas no Google Play / Apple e usar EAS Build (passo a passo).
