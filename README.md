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

Recentemente, concluímos uma intervenção profunda num projeto de Educação Financeira em Realidade Virtual. O objetivo foi elevar o projeto de um estado técnico instável para uma experiência imersiva polida, corrigindo bugs críticos de física e ambiente.

Aqul estão as principais melhorias implementadas:

1. Saúde Técnica e Compilação

Restaurámos a fundação do projeto que estava comprometida por erros de referência.





Sincronização de GUIDs: Corrigimos objetos com "Missing Script" (como o GoalManager) através da edição manual de metadados (.meta), garantindo que a Unity reconhece todos os componentes.



Resolução de Conflitos: Eliminámos scripts duplicados, garantindo uma compilação 100% limpa.

2. Aperfeiçoamento do Player Controller

O controlo do jogador foi totalmente refinado para garantir conforto e realismo.





Tamanho do Jogador: Ajustámos a escala e altura do XR Origin para que a perspetiva no mundo VR seja natural e proporcional ao cenário.



Velocidade e Locomoção: Aumentámos a velocidade de movimento de 2.5 para 5.0, tornando a navegação pela cidade muito mais fluida.



Correção do Jump Infinito: Resolvemos um bug crítico na física que permitia salts ilimitados. Agora, o sistema de salto respeita as colisões com o chão, impedindo o "voo" indesejado do jogador.

3. Sistema de NPCs e Decisões

O coração do jogo a interação social foi estabilizado.





Posicionamento Inteligente: Corrigimos a posição de spawn dos NPCs para garantir que não aparecem dentro de objetos ou em locais inacessíveis.



Gatilhos de Decisão: Refatorámos os scripts de interação. Agora, ao aproximar-se de um NPC, o menu de decisões financeiras ativa-se instantaneamente e sem falhas.

4. Ambiente Visual: Céu e Nevoeiro (Fog)

O aspeto visual do jogo foi transformado para remover artefactos estranhos.





Céu (Skybox): Substituímos o céu amarelo saturado por um Skybox equilibrado e realista.



Ajuste de Fog: Configurámos o nevoeiro ambiental para dar profundidade à cidade sem esconder os objetivos, criando uma atmosfera visualmente apelativa e profissional.

5. Novas Mecânicas de Exploração (Sistema de Táxi)

Adicionámos conveniência à exploração urbana.





Fast Travel: Implementámos um Prefab de Táxi. Quando o jogador interage com o veículo, surge um menu de transporte rápido que permite voltar para casa num clique, otimizando o fluxo entre missões.

6. Auditoria de Estabilidade

Realizámos uma análise profunda ao código YAML da cena para garantir que não existem referências fantasma. Todas as dependências agora apontam para componentes oficiais da Unity ou scripts validados.

Conclusão: O jogo está agora num estado de "produção pronta". Com a física do salto corrigida, a velocidade otimizada, o ambiente visual limpo e os NPCs a funcionar corretamente, o projeto oferece agora uma experiência de Realidade Virtual robusta para o ensino de literacia financeira.


