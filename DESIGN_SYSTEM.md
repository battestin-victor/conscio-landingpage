# 📐 Conscio. Design System (v1.0)

> **"Consistência gera Confiança."**

Este documento define as regras visuais e comportamentais da interface do Conscio. O objetivo é manter uma experiência de usuário (UX) coesa, profissional e focada na redução da carga cognitiva do contador.

---

## 1. Tipografia (Typography)
A escolha tipográfica equilibra a personalidade moderna da marca com a legibilidade necessária para dados financeiros densos.

### Primária (Display & Headings)
* **Família:** `Montserrat`
* **Uso:** Logos, Títulos de Seção, Números Grandes (KPIs), Botões Principais.
* **Pesos:**
    * **Bold (700) / ExtraBold (800):** Para impacto e hierarquia forte.
    * **SemiBold (600):** Subtítulos.

### Secundária (Body & Interface)
* **Família:** `Inter` (ou `Roboto` como fallback)
* **Uso:** Textos corridos, Labels de formulários, Tabelas de dados, Tooltips.
* **Pesos:**
    * **Regular (400):** Leitura geral.
    * **Medium (500):** Ênfase em dados e cabeçalhos de tabela.

### Técnica (Code & Logs)
* **Família:** `JetBrains Mono`, `Fira Code` ou `Consolas`.
* **Uso:** O terminal de logs, chaves de acesso, XMLs brutos.
* **Por que:** Fontes monoespaçadas garantem que cada caractere ocupe o mesmo espaço, facilitando a identificação de erros em chaves fiscais.

---

## 2. Paleta de Cores Expandida (Color System)

Não usamos cores aleatórias. Cada tom tem uma função semântica na interface.

### 🌑 Superfícies (Dark Theme Base)
Onde o conteúdo vive. A profundidade é criada através de variações de luminosidade, não de sombras pesadas.

| Token | Hex | Aplicação |
| :--- | :--- | :--- |
| `surface-deep` | **`#0F2027`** | **Fundo Global.** A base da aplicação. Profundo, reduz brilho excessivo. |
| `surface-card` | **`#182B34`** | **Containers/Cards.** Áreas onde o usuário insere dados. |
| `surface-hover`| **`#203642`** | **Estados Interativos.** Hover em linhas de tabela ou cards. |

### ⚡ Marca & Ação (Brand)
| Token | Hex | Aplicação |
| :--- | :--- | :--- |
| `brand-primary`| **`#6C5CE7`** | **Electric Indigo.** Botões principais (CTA), Links, Ponto do Logo. |
| `brand-hover`  | **`#5849BE`** | Estado de hover do botão principal. |
| `brand-glow`   | `rgba(108, 92, 231, 0.15)` | Efeitos de luz/sombra colorida sutis. |

### 🚦 Semântica (Feedback)
Crucial para softwares fiscais. O usuário precisa saber instantaneamente se a nota foi processada ou falhou.

| Token | Hex | Significado | Aplicação |
| :--- | :--- | :--- | :--- |
| `state-success`| **`#00E676`** | **Sucesso.** | Log: "Nota processada", "Conexão OK". |
| `state-error`  | **`#FF5252`** | **Erro Crítico.** | Log: "Falha SOAP", "Certificado Vencido". |
| `state-warning`| **`#FFAB40`** | **Atenção.** | Log: "Nota sem retenção", "Tempo limite próximo". |
| `state-info`   | **`#40C4FF`** | **Informação.** | Log: "Buscando dados...", "Aguardando". |

### 📝 Texto & Conteúdo
| Token | Hex | Aplicação |
| :--- | :--- | :--- |
| `text-high`    | **`#F5F7FA`** | **Títulos e Dados.** Contraste máximo para leitura (Off-White). |
| `text-medium`  | **`#A0AAB5`** | **Labels e Descrições.** Reduz o ruído visual. |
| `text-disabled`| **`#546E7A`** | **Placeholder/Inativo.** Botões desabilitados. |

---

## 3. Componentização & Física (UI Rules)

### Bordas & "Squircles"
Não somos quadrados (velhos), nem redondos demais (infantis).
* **Border Radius Padrão:** `8px` (Inputs, Botões pequenos).
* **Border Radius Cards:** `12px` ou `16px` (Cards grandes, Modais).
* **Conceito:** Suavidade tecnológica.

### Espaçamento (Grid de 4px)
Para manter o alinhamento perfeito, usamos múltiplos de 4.
* **Margens Pequenas:** `4px`, `8px` (distância entre label e input).
* **Margens Médias:** `16px`, `24px` (distância entre elementos internos do card).
* **Margens Grandes:** `32px`, `40px` (distância entre seções).

### Feedback Visual (Affordance)
* **Botões:** Devem ter um estado de *Hover* (mudança de cor) e *Active* (leve "afundamento" ou clique).
* **Loading:** Nunca deixe a interface congelada. Use *Skeleton Screens* (esqueletos cinzas pulsando) ou *Spinners* Roxo/Indigo para indicar processamento.

---

*Este Design System é um organismo vivo. Mantenha-o atualizado conforme o produto evolui.*
