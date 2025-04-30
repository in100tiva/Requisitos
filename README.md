# Proposta de Valor: Sistema de Gestão de Solicitações de Compra

## 1. Visão Geral do Projeto

O sistema de gestão de solicitações de compra visa automatizar e otimizar o processo de requisições, aprovações e acompanhamento de solicitações de compra dentro da organização. Com base nas 17 funções definidas, o sistema oferecerá:

- Autenticação e controle de acesso com diferentes níveis de usuário
- Fluxo completo de solicitações de compra, desde a criação até a aprovação
- Gerenciamento documental com anexos
- Segurança avançada com JWT e registro de logs
- Interface intuitiva para visualização e gerenciamento de solicitações

## 2. Classificação das Funções por Complexidade

Abaixo, classificamos cada uma das 17 funções do sistema quanto ao seu nível de complexidade:

| Função | Complexidade | Justificativa |
|--------|-------------|---------------|
| 1. Login de Usuário | Simples | Funcionalidade padrão com implementação bem estabelecida em Django |
| 2. Validação de Usuário no Banco | Simples | Verificação básica de credenciais contra o banco de dados |
| 3. Controle de Níveis de Acesso | Média | Requer implementação de permissões e regras específicas |
| 4. Carregar Dados do Usuário no Login | Simples | Consulta simples ao banco para carregar perfil do usuário |
| 5. Fluxo de Aprovação de Solicitação | Complexa | Envolve regras de negócio complexas e múltiplos estados |
| 6. Consulta de Solicitações Pendentes para Aprovação | Média | Requer filtros específicos e interface de apresentação |
| 7. Aprovar ou Reprovar Solicitação com Comentário | Média | Envolve atualizações de status e registro de justificativas |
| 8. Gerenciamento de Sessão Segura (JWT) | Complexa | Implementação de segurança avançada com token e expiração |
| 9. Registro de Logs de Ações | Média | Sistema de auditoria para rastrear ações dos usuários |
| 10. Abrir Nova Solicitação de Compra | Média | Formulário complexo com múltiplos campos e validações |
| 11. Buscar Solicitações Existentes | Simples | Consulta ao banco com filtros básicos |
| 12. Visualizar Solicitações por Status | Simples | Agrupamento e exibição de dados por categoria |
| 13. Atualizar Status de Solicitação | Média | Validações de permissão e atualização de estado |
| 14. Editar Solicitação de Compra | Média | Formulário com validações e verificações de permissão |
| 15. Excluir Solicitação de Compra | Média | Verificações de permissão e exclusão lógica |
| 16. Anexar Documento em Solicitação | Complexa | Upload, armazenamento e gerenciamento de arquivos |
| 17. Gerar Número Automático de Solicitação | Simples | Algoritmo simples de geração sequencial ou customizada |

**Resumo:**
- Funções Simples: 6 funções
- Funções de Complexidade Média: 8 funções
- Funções Complexas: 3 funções

## 3. Estimativa de Custo por Nível de Desenvolvedor

Com base na classificação acima, apresentamos a estimativa de custo detalhada por nível de desenvolvedor:

### 3.1 Desenvolvedor Júnior

| Complexidade | Quantidade | Valor Unitário | Subtotal |
|--------------|------------|----------------|----------|
| Simples | 6 | R$ 1.000 | R$ 6.000 |
| Média | 8 | R$ 2.200 | R$ 17.600 |
| Complexa | 3 | R$ 3.500 | R$ 10.500 |
| **TOTAL** | **17** | | **R$ 34.100** |

**Faixa de preço estimada:** R$ 30.000 - R$ 40.000

### 3.2 Desenvolvedor Pleno

| Complexidade | Quantidade | Valor Unitário | Subtotal |
|--------------|------------|----------------|----------|
| Simples | 6 | R$ 1.800 | R$ 10.800 |
| Média | 8 | R$ 3.500 | R$ 28.000 |
| Complexa | 3 | R$ 6.000 | R$ 18.000 |
| **TOTAL** | **17** | | **R$ 56.800** |

**Faixa de preço estimada:** R$ 50.000 - R$ 65.000

### 3.3 Desenvolvedor Sênior

| Complexidade | Quantidade | Valor Unitário | Subtotal |
|--------------|------------|----------------|----------|
| Simples | 6 | R$ 3.000 | R$ 18.000 |
| Média | 8 | R$ 5.500 | R$ 44.000 |
| Complexa | 3 | R$ 9.500 | R$ 28.500 |
| **TOTAL** | **17** | | **R$ 90.500** |

**Faixa de preço estimada:** R$ 85.000 - R$ 110.000

## 4. Estimativa de Tempo por Nível de Desenvolvedor

### 4.1 Desenvolvedor Júnior

| Complexidade | Quantidade | Dias por Função | Subtotal (dias) |
|--------------|------------|-----------------|----------------|
| Simples | 6 | 4 | 24 |
| Média | 8 | 8 | 64 |
| Complexa | 3 | 13 | 39 |
| **TOTAL** | **17** | | **127 dias** |

**Prazo total estimado:** 25-26 semanas (aproximadamente 6 meses)

### 4.2 Desenvolvedor Pleno

| Complexidade | Quantidade | Dias por Função | Subtotal (dias) |
|--------------|------------|-----------------|----------------|
| Simples | 6 | 2 | 12 |
| Média | 8 | 5 | 40 |
| Complexa | 3 | 8 | 24 |
| **TOTAL** | **17** | | **76 dias** |

**Prazo total estimado:** 15-16 semanas (aproximadamente 4 meses)

### 4.3 Desenvolvedor Sênior

| Complexidade | Quantidade | Dias por Função | Subtotal (dias) |
|--------------|------------|-----------------|----------------|
| Simples | 6 | 1 | 6 |
| Média | 8 | 3 | 24 |
| Complexa | 3 | 6 | 18 |
| **TOTAL** | **17** | | **48 dias** |

**Prazo total estimado:** 10 semanas (aproximadamente 2,5 meses)

## 5. Análise Comparativa

### 5.1 Comparativo de Custo-Benefício

| Nível | Custo Total | Prazo (meses) | Custo Médio Mensal | Custo por Função |
|-------|------------|---------------|-------------------|------------------|
| Júnior | R$ 34.100 | 6 | R$ 5.683 | R$ 2.006 |
| Pleno | R$ 56.800 | 4 | R$ 14.200 | R$ 3.341 |
| Sênior | R$ 90.500 | 2,5 | R$ 36.200 | R$ 5.324 |

### 5.2 Considerações Importantes

#### Desenvolvedor Júnior:
- **Vantagens**: Menor custo inicial
- **Desvantagens**: Prazo mais longo, maior probabilidade de retrabalho, necessidade de supervisão, implementação potencialmente menos robusta

#### Desenvolvedor Pleno:
- **Vantagens**: Bom equilíbrio entre custo e prazo, conhecimento suficiente para implementar todas as funções com qualidade
- **Desvantagens**: Pode necessitar de consulta em funções mais complexas

#### Desenvolvedor Sênior:
- **Vantagens**: Entrega mais rápida, código de maior qualidade e manutenibilidade, menor risco de retrabalho
- **Desvantagens**: Custo inicial mais elevado

## 6. Benefícios do Sistema

### 6.1 Benefícios Estratégicos
- Otimização do processo de compras
- Governança e compliance
- Visibilidade e controle
- Redução de erros e retrabalho

### 6.2 Benefícios Operacionais
- Centralização da informação
- Rastreabilidade completa
- Agilidade na aprovação
- Organização documental

### 6.3 Diferenciais Técnicos
- Segurança avançada
- Interface intuitiva
- Escalabilidade
- Geração automática de números

## 7. Recomendação Final

Considerando a natureza do sistema, que envolve fluxos de aprovação, segurança e gerenciamento de documentos, recomendamos a contratação de um **desenvolvedor pleno**.

Esta opção oferece o melhor equilíbrio entre custo, prazo e qualidade. Um desenvolvedor pleno possui conhecimento técnico suficiente para implementar as funções complexas com qualidade adequada, sem o custo elevado de um desenvolvedor sênior.

Para um projeto crítico que exija máxima qualidade e velocidade de implementação, um desenvolvedor sênior seria a escolha ideal, apesar do custo mais elevado.

*Esta proposta considera apenas o desenvolvimento das funcionalidades listadas. Custos adicionais podem incluir: infraestrutura, treinamento, suporte e manutenção pós-implementação.*
