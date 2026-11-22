JEJUM DE DESESPERO — pacote pronto para Vercel

Conteúdo:
- index.html: app estática autónoma (cartaz e fotografia incorporados)
- cartaz_jejum_de_desespero.jpg
- fotografia_silvia.jpg

PUBLICAÇÃO MAIS SIMPLES (sem código):
1. Acede a https://vercel.com/new e inicia sessão/cria conta.
2. Para publicar por Git, cria um repositório e coloca estes ficheiros na raiz; importa o repositório na Vercel.
   Framework Preset: Other (ou None)
   Build Command: deixa vazio / Override desligado
   Output Directory: . (ou deixa a deteção automática)
3. Deploy. A Vercel dará um endereço público *.vercel.app.
4. Abre o endereço no telemóvel e testa antes de partilhar.

ALTERNATIVA COM CLI (se tiveres Node.js instalado):
- Abre Terminal/PowerShell nesta pasta.
- Executa: npx vercel
- Segue as perguntas, escolhe Other/Static e confirma a pasta atual como raiz.
- Para publicar em produção: npx vercel --prod

NOTAS:
- App estática; não requer dependências nem comando de build.
- Dia 1 é pré-visualizável; calendário começa em 22/12/2026 e os dias seguintes abrem por data local do dispositivo.
- Não existe bloqueio robusto no servidor: mudar a data/hora do dispositivo pode antecipar desbloqueios.
- Diário/progresso ficam guardados no navegador/dispositivo. Não há sincronização com a organizadora.
- O botão WhatsApp abre mensagem preparada; a participante tem de enviar.


A mini-app inclui agora uma secção de instruções de instalação no telemóvel (Android/Chrome e iPhone/Safari), visível na própria página.


INSCRICAO POR EMAIL
A página de entrada pede nome, email, telemóvel e consentimento. Ao enviar, os dados são submetidos ao FormSubmit para info@afabricadafelicidade.com com assunto "Inscrição Jornada do Desespero". O FormSubmit pode exigir que a proprietária confirme/ative o destinatário no primeiro envio antes de os emails começarem a chegar. Teste primeiro com uma inscrição real.
O formulário usa um serviço externo; os dados pessoais são transmitidos a esse fornecedor. A caixa de consentimento e a informação de privacidade devem ser revistas antes de divulgar. A inscrição é guardada localmente no navegador para não voltar a mostrar o formulário nesse dispositivo.

ATUALIZAÇÃO: INSTALAÇÃO POR BOTÃO
- A aplicação inclui manifest.webmanifest, service worker e ícones PWA.
- Os botões “Instalar no telemóvel” tentam abrir a instalação nativa quando suportada.
- Em iPhone, ou quando a instalação nativa não está disponível, o botão apresenta instruções para adicionar ao ecrã principal.
- Publica todos os ficheiros e pastas, incluindo /icons, /manifest.webmanifest e /sw.js.
