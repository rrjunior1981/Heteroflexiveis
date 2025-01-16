!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portal Heteroflexíveis</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom, #ff8c00, #ff6347);
      color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .container {
      text-align: center;
      padding: 20px;
      width: 90%;
    }
    h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
      color: #fff;
      text-shadow: 2px 2px 5px #000;
    }
    h2 {
      font-size: 1.5em;
      margin-bottom: 20px;
      color: #ffebcd;
    }
    #countdownBox {
      background-color: rgba(0, 0, 0, 0.7);
      padding: 20px;
      border-radius: 10px;
      margin: 20px 0;
      text-align: center;
    }
    #countdown {
      font-size: 2.2em;
      font-family: 'Courier New', monospace;
      color: #00ff7f;
    }
    .button {
      background-color: #ffffff;
      color: #000000;
      border: none;
      padding: 15px 30px;
      margin: 10px;
      border-radius: 10px;
      font-size: 1.2em;
      cursor: pointer;
      transition: background-color 0.3s;
      box-shadow: 2px 2px 8px rgba(0, 0, 0, 0.5);
    }
    .button:hover {
      background-color: #000000;
      color: #ffffff;
    }
    .output-box {
      background-color: rgba(0, 0, 0, 0.8);
      color: #ffebcd;
      padding: 20px;
      margin-top: 20px;
      border-radius: 10px;
      font-size: 1.5em;
      text-align: center;
      width: 90%;
      box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.6);
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Portal Heteroflexíveis</h1>
    <h2>Convenção Lundbeck Sem Régis Alagoas 2025</h2>

    <div id="countdownBox">
      <div id="countdown">00d 00h 00m 00s</div>
    </div>

    <button class="button" onclick="generatePhrase('impact')">Gerar Frase de Impacto Plenária</button>
    <button class="button" onclick="generatePhrase('escape')">Gerar Desculpa Fugir Papo Merda</button>
    <button class="button" onclick="generatePhrase('challenge')">Desafio Aleatório</button>

    <div id="output" class="output-box"></div>
  </div>

  <script>
    // Configuração do contador
    const targetDate = new Date();
    targetDate.setDate(targetDate.getDate() + ((7 - targetDate.getDay()) % 7));
    targetDate.setHours(12, 0, 0, 0);

    const countdownEl = document.getElementById("countdown");

    function updateCountdown() {
      const now = new Date();
      const timeLeft = targetDate - now;

      const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
      const hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((timeLeft % (1000 * 60)) / 1000);

      countdownEl.textContent = `${days}d ${hours}h ${minutes}m ${seconds}s`;
    }

    setInterval(updateCountdown, 1000);
    updateCountdown();

    // Frases e desafios
    const phrases = {
      impact: [
        "Venda é como um bom remédio: na dose certa, cura tudo.",
        "Se até o antidepressivo tem efeito prolongado, sua persistência também pode ter.",
        "A meta não é um limite, é só um número pra começar a conversa.",
        "Se a Lundbeck acredita na gente, quem somos nós para duvidar?",
        "Convencendo médicos ou chefes, a arte da venda é universal.",
        "Venda como se o bônus dependesse do próximo café.",
        "Cliente difícil é igual a bula: parece complicado, mas a gente domina.",
        "A melhor prescrição é saber ouvir antes de falar.",
        "Seja como um ISRS: comece devagar, mas conquiste resultados sólidos.",
        "Seu território não tem limites, só oportunidades.",
        "Persista mais do que o tratamento contínuo.",
        "Venda é como marketing farmacêutico: tudo está na comunicação.",
        "Foco no cliente certo: não adianta empurrar antipsicótico pra quem só precisa de café.",
        "A meta é o diagnóstico inicial, mas a alta é sempre maior.",
        "Seja o melhor vendedor, mesmo se só tiver genéricos ao redor.",
        "O paciente precisa do tratamento, mas o médico precisa de você.",
        "Venda é ciência e arte: estude os dois.",
        "Dê ao cliente o que ele não sabia que precisava, como uma boa analogia.",
        "A concorrência é o placebo, você é o tratamento certo.",
        "Não trate objeções como efeito colateral: trate como chance de sucesso."
      ],
      escape: [
        "Preciso levar minha avó pro taekwondo.",
        "Volto já, preciso resgatar meu gato que ficou preso no micro-ondas.",
        "O Josiel está me ligando no Teams pra falar da meta de 2030.",
        "Desculpa, esqueci minha colher de sopa na sala de café.",
        "Preciso pegar o relatório que mandei errado pro gerente do Libbs.",
        "Gente, minha geladeira está piscando. Alguém sabe se isso é normal?",
        "Esqueci o modem ligado, vai que explode.",
        "Meu vizinho pediu ajuda com uma oferta de Brintellix genérico, volto já.",
        "Preciso fazer uma ligação urgente pro meu veterinário.",
        "Minha mãe ligou falando que o cachorro entrou no Uber sozinho.",
        "Volto já, o Josiel pediu pra buscar a chave da sala.",
        "Preciso resolver um problema com o GPS que tá me mandando pro Polo Norte.",
        "Esqueci de tomar meu placebo hoje, já volto.",
        "Tá dando um bug no meu relógio biológico, vou dar uma pausa.",
        "Meu psiquiatra pediu pra eu evitar papos sem ROI, então preciso ir.",
        "Volto já, só vou confirmar se ainda tem pão de queijo na mesa.",
        "Pausa estratégica: vou buscar inspiração no banheiro.",
        "Preciso ir ali ver se a cota já abaixou sozinha.",
        "O cliente acabou de me responder no WhatsApp... Era um 'Oi'.",
        "Volto em 5 minutos. Prometi que ia buscar o Carlão pra abrir a rodada de chopp."
      ],
      challenge: [
        "Mande o Carlão tirar a camisa.",
        "Aperte a bunda do amigo mais próximo.",
        "Faça uma rodada de xote e brinde aos amigos.",
        "Pergunte pro Josiel quando poderemos tirar férias qualquer época do ano.",
        "Pergunte ao seu chefe se tem como liberar o acesso ao Xvideos.",
        "Pegue o copo de bebida da mão do amigo mais próximo e vire tudo sem explicar nada.",
        "Peça para o Júnior fazer uma pergunta.",
        "Chame o Cainho de Paraíba.",
        "Pergunte pra Andréa se vai ter pagode.",
        "Pergunte pra Letícia se faz sentido.",
        "Peça pro Marquinhos abaixar a sua cota.",
        "Chame o Igor de tiozão da Sukita em voz alta.",
        "Faça um discurso motivacional sobre vender gelo no Alasca.",
        "Desafie alguém a pular de costas na piscina.",
        "Crie uma história inventada sobre uma reunião que nunca existiu.",
        "Cumprimente todos na roda dizendo 'bom dia' mesmo que seja à noite.",
        "Pergunte ao organizador se os médicos recebem cashback por receita.",
        "Faça uma dancinha enquanto diz 'sou um ISRS em forma de gente'.",
        "Ofereça vender antidepressivo pro garçom.",
        "Comece a pedir autógrafos dos palestrantes como se fossem celebridades."
      ]
    };

    function generatePhrase(type) {
      const outputEl = document.getElementById("output");
      const randomPhrase = phrases[type][Math.floor(Math.random() * phrases[type].length)];
      outputEl.textContent = randomPhrase;
    }
  </script>
</body>
</html>
