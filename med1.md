```mermaid

graph LR
    %% Nós do modelo
    X[Coping Emocional]
    M["Preferência por<br/>Músicas Reflexivas"]
    Y[Afeto Positivo]
    IE["Efeito Indireto (a×b):<br/><b>0.038***</b>"]

    %% Caminhos com estatísticas (substitua [valor])
    X --> |"a = [valor]"| M
    M --> |"b = [valor]"| Y
    X --> |"c' = 0.208***"| Y

    %% Estilo Vazado (Preto no Branco)
    classDef customStyle fill:#fff,stroke:#000,stroke-width:2px,color:#000
    class X,M,Y customStyle
    style IE fill:#fff,stroke:#ccc,stroke-width:1px,color:#000
    
    %% Estilo das setas e texto (aqui está a solução)
    linkStyle default stroke:#000,stroke-width:1.5px
    %% Força o estilo do texto da seta a ter fundo branco
    style M fill:#fff
    style Y fill:#fff
