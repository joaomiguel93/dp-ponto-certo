# ⏱ PontoCerto DP

> Ferramenta gratuita para apuração de cartão ponto — desenvolvida para contadores e profissionais de Departamento Pessoal.

![Versão](https://img.shields.io/badge/versão-5.0-blue)
![Licença](https://img.shields.io/badge/licença-livre-green)
![Linguagem](https://img.shields.io/badge/linguagem-HTML%20%2F%20CSS%20%2F%20JS-orange)
![CLT](https://img.shields.io/badge/conformidade-CLT%202024-blueviolet)

---

## 📋 Sobre o projeto

O **PontoCerto DP** substitui planilhas manuais e acelera o fechamento de ponto mensal. O contador recebe os dados prontos — horas trabalhadas, extras, atrasos e adicional noturno — organizados conforme a CLT, prontos para lançamento na folha de pagamento.

Desenvolvido com auxílio de inteligência artificial ([Claude / Anthropic](https://www.anthropic.com)).

---

## ✨ Funcionalidades

### Apuração de Ponto
- Tabela mensal gerada automaticamente com todos os dias do mês
- Campos editáveis: Entrada, Saída para intervalo, Retorno do intervalo, Saída final
- Preenchimento automático baseado na jornada padrão configurada
- Navegação rápida entre campos com `Enter` e `Tab`

### Atalhos de teclado na linha
| Tecla | Ação |
|-------|------|
| `F` | Marcar falta |
| `A` | Marcar atestado médico |
| `E` | Marcar feriado |
| `R` | Limpar o dia |

### Cálculos automáticos (CLT)
- **Horas trabalhadas** por dia
- **Horas extras** (50% dias úteis / 100% domingos e feriados) — Art. 59 CLT
- **Horas extras com faixas personalizadas** (modo custom)
- **Atrasos** com tolerância configurável — Art. 58 §1º CLT
- **Adicional noturno** (22h–05h, com hora reduzida de 52'30'') — Art. 73 CLT · Súmula 60 TST
- **Intrajornada** com alerta de violação do intervalo mínimo — Art. 71 CLT · Súmula 437 TST
- Identificação automática de **faltas**, **atestados** e dias incompletos

### Resumo Mensal
- Totais prontos para folha: horas trabalhadas, HE 50%, HE 100%, adicional noturno, atrasos, faltas e atestados
- Referência legal de cada item calculado

### Feriados
- Base de feriados nacionais pré-cadastrada (2025, 2026 e 2027)
- Cadastro de feriados estaduais e municipais
- Marcação automática na tabela de ponto

### Funcionários
- Cadastro de múltiplos funcionários
- Alternância rápida entre funcionários sem perder dados
- Dados salvos automaticamente no navegador (localStorage)

### Exportação
- **CSV** — dados organizados por dia, prontos para importar em qualquer sistema de folha
- **PDF / Impressão** — layout A4 otimizado para impressão

---

## 🏛 Base legal implementada

| Regra | Dispositivo |
|-------|-------------|
| Horas extras | Art. 59 CLT · Súmula 291 TST |
| Tolerância de atraso | Art. 58 §1º CLT |
| Adicional noturno | Art. 73 CLT · Súmula 60 TST |
| Hora noturna reduzida | Art. 73 §1º CLT |
| Intervalo intrajornada | Art. 71 CLT · Súmula 437 TST |
| Faltas e descontos | Art. 131 CLT |
| HE em domingos/feriados | Art. 59 CLT |

---

## 🚀 Como usar

Não requer instalação, servidor ou cadastro.

1. Faça o download do arquivo `ponto-certo.html`
2. Abra no navegador (duplo clique)
3. Configure a jornada padrão, selecione o mês e clique em **Gerar Tabela**
4. Digite os horários linha a linha (ou use **Preencher Padrão**)
5. Exporte o CSV ou imprima o PDF

---

## 💾 Persistência de dados

Os dados dos funcionários e feriados cadastrados são salvos automaticamente no `localStorage` do navegador — ficam disponíveis mesmo após fechar e reabrir a aba.

Os registros de ponto da sessão atual são mantidos por funcionário. Para segurança, **exporte sempre o CSV** antes de fechar o navegador ou limpar o cache.

---

## 🖥 Compatibilidade

Funciona em qualquer navegador moderno sem necessidade de instalação:

- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Safari (macOS / iOS)

---

## 🛠 Tecnologias

Arquivo único `.html` — sem frameworks, sem dependências, sem servidor.

- **HTML5** — estrutura e formulários
- **CSS3** — layout, tema claro/escuro, responsividade
- **JavaScript (ES6+)** — lógica de cálculo CLT, persistência e exportação
- **Google Fonts** — tipografia (DM Sans + DM Mono) — requer conexão à internet; sem conexão, usa fonte padrão do sistema sem impacto funcional

---

## 🔮 Versão PRO — em breve

| Funcionalidade | Versão Gratuita | Versão PRO |
|----------------|:-:|:-:|
| Apuração mensal completa | ✅ | ✅ |
| Múltiplos funcionários | ✅ | ✅ |
| Exportação CSV | ✅ | ✅ |
| Cálculos CLT automáticos | ✅ | ✅ |
| Cadastro persistente (nuvem) | ❌ | ✅ |
| Importação TXT/CSV de relógio | ❌ | ✅ |
| Cálculo de DSR sobre HE | ❌ | ✅ |
| Espelho de ponto assinável em PDF | ❌ | ✅ |
| Login multi-usuário por escritório | ❌ | ✅ |
| Backup em nuvem | ❌ | ✅ |

---

## 📄 Licença

Uso livre para escritórios de contabilidade e profissionais de Departamento Pessoal.  
Redistribuição permitida desde que mantidos os créditos do autor.

---

## 👨‍💻 Autor

**João Miguel E Ferreira**  
📧 contato_joaomiguel@outlook.com.br  
🔗 [github.com/joaomiguel93/dp-ponto-certo](https://github.com/joaomiguel93/dp-ponto-certo)

---

> ⭐ Se esta ferramenta te economizou tempo, deixe uma estrela no repositório e compartilhe com outro profissional de DP!
