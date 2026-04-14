Visão Geral do Projeto

Nome do Projeto: My project (7)

Motor de Jogo: Unity 6 (Versão 6000.2.8f1)

Plataforma Alvo: Android (provavelmente Meta Quest / Oculus)

Idioma: Português (PT-PT/PT-BR)

🎮 Mecânicas de Jogo (Core Loop)

O jogo gira em torno da gestão de dinheiro e tomada de decisões financeiras:

Tarefas Diárias ( C# TaskManager.cs ):

O jogador deve realizar tarefas domésticas para ganhar recompensas.

Exemplos: Lavar a louça, Arrumar o quarto, Regar as plantas, Passear o cão.

Tomada de Decisões ( C# DecisionManager.cs ):

São apresentados dilemas financeiros onde o jogador deve escolher como gastar ou poupar o seu dinheiro.

Exemplos: Comprar um jogo vs um boneco, Snacks na escola vs levar de casa, Fazer um presente vs comprar.

Objetivo Financeiro ( C# FinanceManager.cs ):

O objetivo final é poupar uma quantia específica (ex: 150€) para comprar um item desejado (Sapatilhas).

📁 Estrutura de Pastas Relevante

Assets/Scripts : Contém toda a lógica do jogo (Gestores de tarefas, finanças, NPCs e interações VR).

Assets/scenes : Inclui cenas de Menu Principal, Início e a cena principal de jogo (samplescene).

Assets/XR : Configurações para interação VR (XR Interaction Toolkit).

Assets/Tom's Terrain Tools : Ferramentas para criação de terreno.

🛠️ Tecnologias Utilizadas

XR Interaction Toolkit: Para interações VR.

TextMesh Pro: Para toda a interface de utilizador (UI).

Sistema de Tarefas Aleatórias: Para manter o gameplay dinâmico a cada "dia" no jogo.




