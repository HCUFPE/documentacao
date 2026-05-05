# Modelagem de Casos de Uso

## 1. Diagrama de Casos de Uso
*(Inserir imagem ou Mermaid)*
```mermaid
flowchart LR
    %% Definição dos Atores
    E((Enfermeiro))
    M((Médico))
    
    subgraph "Sistema Hospitalar"
        UC1([Realizar Triagem])
        UC2([Consultar Histórico])
        UC3([Prescrever Medicamento])
    end
    
    %% Relacionamentos
    E --- UC1
    E --- UC2
    M --- UC2
    M --- UC3
```
## 2. Especificação (Exemplo)
### UC001 - Triagem
* **Ator**: Enfermeiro.
* **Fluxo**: Selecionar paciente -> Inserir Sinais Vitais -> Calcular Manchester.
