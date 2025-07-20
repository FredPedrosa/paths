```mermaid

graph LR
    %% Nós do modelo
    X["Coping Emocional"]
    M["Preferência por<br/>Músicas Reflexivas"]
    Y["Afeto Positivo"]
    IE["Efeito Indireto (a×b) = <br/><b>0.038***</b>"]

    %% Caminhos com estatísticas (lembre-se de substituir [valor])
    X --> |"a = [valor]"| M
    M --> |"b = [valor]"| Y
    X --> |"c' = 0.208***"| Y

    %% Estilo Vazado (Preto no Branco)
    classDef customStyle fill:#fff,stroke:#000,stroke-width:2px,color:#000
    class X,M,Y customStyle
    
    %% Estilo da nota do efeito indireto
    style IE stroke-width:2px,fill:#fff,color:#000
    
    %% Estilo das setas e texto
    linkStyle default stroke:#000,color:#000,stroke-width:1.5px
