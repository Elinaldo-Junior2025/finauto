# PRD - FinAuto MVP

## 1. Visão Geral

O FinAuto é um aplicativo simples de controle financeiro pessoal que permite aos usuários importar extratos bancários (CSV e PDF estruturado) e visualizar rapidamente seus gastos através de um dashboard intuitivo. O foco está na facilidade de uso e na classificação automática de despesas.

## 2. Problema

Usuários enfrentam dificuldades comuns no controle financeiro:
- Registrar manualmente todos os gastos consome tempo
- Classificar despesas de forma consistente é trabalhoso
- Entender padrões de consumo sem visualização clara dos dados
- Falta de ferramentas simples que não exigem integração bancária complexa

## 3. Solução (MVP)

O MVP do FinAuto oferece:

1. **Importação de arquivos**: CSV e PDF estruturado (sem OCR)
2. **Extração automática**: data, descrição e valor das transações
3. **Classificação automática**: baseada em palavras-chave predefinidas
4. **Edição e exclusão**: ajuste manual de transações importadas
5. **Dashboard mensal básico**: visualização de gastos, receitas e categorias

## 4. Escopo do MVP

### Inclui:
- Cadastro simples de usuário
- Importação de extratos em CSV e PDF estruturado
- Classificação automática por palavras-chave
- Edição e exclusão de transações
- Dashboard com resumo mensal

### Exclui:
- OCR para PDFs não estruturados
- Integração direta com APIs bancárias
- IA avançada para classificação
- Processo de KYC (Know Your Customer)
- Exportação de relatórios complexos
- Múltiplas contas bancárias

## 5. Fluxos Principais

### 5.1 Importar Extrato
1. Usuário envia arquivo (CSV ou PDF estruturado)
2. Sistema lê e extrai colunas (data, descrição, valor)
3. Sistema classifica automaticamente por palavras-chave
4. Usuário revisa transações importadas
5. Dashboard é atualizado com novos dados

### 5.2 Ajustar Categoria
1. Usuário seleciona transação no dashboard
2. Usuário altera a categoria manualmente
3. Sistema oferece opção de aplicar regra para futuras transações similares
4. Dashboard reflete a mudança imediatamente

### 5.3 Dashboard
1. Usuário acessa a tela principal
2. Sistema exibe resumo mensal (gastos totais, receitas, saldo)
3. Usuário visualiza gráfico de gastos por categoria
4. Usuário pode filtrar por categorias específicas

## 6. Regras de Negócio

- Sem necessidade de KYC ou verificação de identidade
- Apenas CSV e PDF estruturado são aceitos (formatos claros com colunas definidas)
- Categorias fixas predefinidas: Alimentação, Transporte, Moradia, Saúde, Lazer, Educação, Outros
- Classificação automática baseada em dicionário de palavras-chave
- Usuário pode editar qualquer transação a qualquer momento
- Dados são armazenados localmente ou em backend seguro (sem compartilhamento)

## 7. Requisitos Não Funcionais

- **Interface**: simples, intuitiva e responsiva (mobile-first)
- **Performance**: importação de até 1000 transações em menos de 5 segundos
- **Segurança**: dados criptografados em repouso e em trânsito
- **Privacidade**: dados do usuário não são compartilhados com terceiros
- **Compatibilidade**: funciona em navegadores modernos (Chrome, Firefox, Safari, Edge)

## 8. Métricas de Sucesso

- Número de importações concluídas com sucesso
- Percentual de classificações automáticas aceitas pelos usuários
- Número médio de correções manuais por importação
- Taxa de retenção de usuários (retorno após 7 e 30 dias)
- Tempo médio para completar primeira importação

## 9. Riscos e Mitigações

### Riscos:
- **Formatos de extrato inconsistentes**: diferentes bancos usam layouts variados
- **Classificação automática limitada**: regras simples podem não cobrir todos os casos

### Mitigações:
- Fornecer orientação clara sobre formato CSV esperado
- Permitir edição rápida e intuitiva de classificações incorretas
- Coletar feedback sobre formatos de extrato mais utilizados para futuras melhorias

---

**Versão**: 1.0  
**Data**: Dezembro 2024  
**Status**: Aprovado para desenvolvimento do MVP
