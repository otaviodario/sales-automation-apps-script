# E-commerce Sales Automation - Google Apps Script

Sistema integrado de automação para gerenciamento de vendas em Google Sheets. Oferece ferramentas para atualização de status de pedidos, geração de relatórios, padronização de dados, cálculo de métricas operacionais e análise financeira. Projetado para operações de e-commerce no mercado brasileiro, com suporte a vendas em marketplaces, WhatsApp e loja física.

## Funcionalidades Principais

- **Gerenciamento de Status**  
  Atualizações automáticas ou manuais para etapas como "NF Impressa", "NF Entregue", "Despachado" e "Cancelado". Inclui remoção de prazos, envio de notificações por e-mail e formatação visual (ex.: cinza para cancelados).

- **Relatórios e Análises**  
  Geração de relatórios de entregas pendentes, produtos vendidos por mês/segmento, churn e SLA semestrais, comparativos mensais de vendas (totais, cancelados, diferenças de frete). Suporte a gráficos sincronizados e projeções baseadas em médias diárias.

- **Padronização de Dados**  
  Normalização de nomes de produtos, cidades/estados (formato "Cidade - UF"), transportadoras e endereços em uma linha. Limites de caracteres com destaque visual, ordenação alfabética de estoque e verificação de valores.

- **Controle de Estoque e Produtos**  
  Destaque para estoque mínimo, listagem de pendências e exclusão de itens comuns em relatórios.

- **Cotações e Fretes**  
  Geração de cotações dinâmicas para transportadoras, comparativos por linha e destaque de divergências entre frete pago e tabelado.

- **Utilitários Adicionais**  
  Criação de abas mensais sequenciais a partir de modelo, inserção de números de linha (ROW), rolagem para última linha vazia, listagem de feriados com formatação e verificação de prazos operacionais.

Interface via menus customizados ("Executar Scripts") e triggers automáticos (onEdit/onOpen) para eficiência diária.

## Por que Utilizar?

Reduz tempo em tarefas repetitivas, como atualizações de status e análises de desempenho. Fornece insights acionáveis para decisões em vendas, logística e finanças, com foco em escalabilidade para operações de médio porte.

## Requisitos

- Conta Google Sheets.  
- Acesso a Extensões > Apps Script para configuração.

## Instalação

1. Crie uma planilha no Google Sheets.  
2. Acesse Extensões > Apps Script e configure o projeto.  
3. Implemente as funções nos arquivos .gs correspondentes.  
4. Execute `onOpen()` para gerar os menus.  
5. Crie abas mensais e configure cabeçalhos padrão.

## Configurações e Personalizações

- Abas ignoradas: arrays como `IGNORE_SHEETS` para excluir relatórios de abas específicas.  
- Cores e limites: hex codes para destaques (ex.: cinza para cancelados) e limites como 255 caracteres.  
- Mapeamentos: dicionários para transportadoras, correções de nomes e origens.  
- E-mails: configure destinatários para notificações de cancelamentos.  
- Datas e meses: adapte para anos/meses personalizados em funções como churn/SLA.

## Compatibilidade e Limitações

Testado em 2025/2026 no Google Sheets. Dependente de formatos consistentes de dados; limites do Sheets aplicam-se a volumes altos. Sem integrações externas nativas.

## Licença

MIT – Livre para uso e modificação interna, sem garantia.

Desenvolvido por Otávio Dario  
LinkedIn: https://www.linkedin.com/in/otaviodario/  
Aberto a contribuições via issues. Versão: fevereiro 2026.
