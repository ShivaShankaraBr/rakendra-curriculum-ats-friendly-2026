# PRD — Rakendra Curriculum ATS Friendly 2026

**Versão:** 1.0  
**Status:** Planejamento do MVP  
**Autor:** Luiz Henrique Camacho Correra (Shiva Shankara)  
**Projeto:** Desafio de Vibe Coding da Digital Innovation One  
**Plataforma de construção:** Lovable

## 1. Visão do produto

O Rakendra Curriculum ATS Friendly 2026 é uma aplicação web que auxilia candidatos a adaptar currículos para vagas específicas. O produto compara o conteúdo fornecido pelo usuário com a descrição da vaga, apresenta uma estimativa de compatibilidade e gera uma versão editável e adequada à leitura por sistemas ATS.

## 2. Problema

Muitos candidatos possuem experiência compatível com uma vaga, mas apresentam o currículo com estrutura difícil de interpretar, linguagem genérica ou ausência de palavras-chave relevantes. Isso pode reduzir a visibilidade da candidatura antes da avaliação humana.

## 3. Objetivo geral

Criar um MVP acessível e direto que ajude o usuário a compreender a aderência entre seu perfil e uma vaga e a produzir um currículo ATS Friendly sem inventar informações.

## 4. Objetivos específicos

- comparar currículo e vaga;
- apresentar pontuação estimada de compatibilidade;
- identificar termos encontrados e ausentes;
- sugerir melhorias de conteúdo e estrutura;
- gerar currículo adaptado e editável;
- exportar currículo em PDF;
- documentar e exportar o design system em PDF;
- funcionar sem login, backend ou chave de API.

## 5. Público-alvo

- pessoas procurando emprego;
- profissionais em transição de carreira;
- estudantes buscando estágio ou primeira oportunidade;
- candidatos que desejam personalizar o currículo por vaga;
- usuários com pouco conhecimento sobre sistemas ATS.

## 6. Proposta de valor

Transformar a descrição de uma vaga e o histórico real do usuário em orientações claras e em um currículo simples, legível e direcionado, sem prometer aprovação e sem fabricar qualificações.

## 7. Escopo do MVP

1. Tela inicial e explicação curta.
2. Entrada do currículo ou perfil profissional.
3. Entrada da descrição da vaga.
4. Análise estimada de compatibilidade.
5. Lista de palavras-chave presentes e ausentes.
6. Recomendações de melhoria.
7. Gerador e editor de currículo.
8. Exportação do currículo em PDF.
9. Página de design system.
10. Exportação do design system em PDF.
11. Dados de demonstração.
12. Persistência local temporária.

## 8. Fora do escopo

- login e cadastro;
- banco de dados em nuvem;
- candidatura automática;
- coleta de vagas externas;
- integração paga com modelos de IA;
- garantia de aprovação em processos seletivos;
- invenção de experiências, cursos ou habilidades.

## 9. Fluxo principal

1. O usuário acessa a aplicação.
2. Seleciona Começar análise.
3. Cola seu currículo ou perfil.
4. Cola a descrição da vaga.
5. Solicita a análise.
6. Visualiza pontuação, correspondências e lacunas.
7. Gera uma versão adaptada.
8. Revisa e edita o conteúdo.
9. Exporta o currículo em PDF.

## 10. Requisitos funcionais

- **RF01:** permitir acesso direto sem autenticação.
- **RF02:** receber currículo e descrição da vaga em campos separados.
- **RF03:** validar que os dois campos possuem conteúdo.
- **RF04:** calcular pontuação estimada entre 0 e 100.
- **RF05:** classificar o resultado em Match forte, Bom potencial ou Risco de ghosting pelo ATS.
- **RF06:** listar palavras-chave encontradas e ausentes.
- **RF07:** apresentar recomendações práticas.
- **RF08:** gerar currículo estruturado usando somente dados informados.
- **RF09:** permitir editar o currículo gerado.
- **RF10:** permitir copiar o currículo.
- **RF11:** exportar o currículo em PDF.
- **RF12:** disponibilizar exemplos para demonstração.
- **RF13:** apresentar o design system.
- **RF14:** exportar o design system em PDF.
- **RF15:** permitir reiniciar a análise sem recarregar a aplicação.

## 11. Requisitos não funcionais

- interface responsiva a partir de 360 px;
- português brasileiro;
- componentes shadcn/ui;
- acessibilidade por teclado e foco visível;
- contraste adequado;
- desempenho compatível com navegadores modernos;
- ausência de erros de TypeScript;
- funcionamento sem backend;
- mensagens transparentes sobre análise estimada.

## 12. Regra de pontuação do MVP

A pontuação pode ser calculada localmente a partir de termos normalizados presentes na vaga e no currículo. A interface deve explicar que o resultado é uma estimativa educativa. Deve haver pesos para palavras-chave, competências técnicas, formação, experiência e estrutura, com limite total de 100 pontos.

## 13. Currículo ATS Friendly

O PDF deve utilizar uma coluna, fundo branco, texto escuro, títulos simples, tipografia legível e seções tradicionais. Não deve depender de ícones, imagens, tabelas complexas, caixas laterais ou elementos que prejudiquem a extração do texto.

## 14. Identidade visual

Base Rakendra: grafite #111311, superfície #1B1E1C, marfim #F6F2E9, dourado #D4A83F e verde #2FA85B. Azul e amarelo-claro devem aparecer somente em detalhes menores. O logotipo oficial deve preservar a lua cheia.

## 15. Critérios de aceitação

1. O app abre sem solicitar login.
2. Os campos aceitam currículo e vaga.
3. A análise não inicia com campos vazios.
4. O resultado apresenta pontuação e justificativa.
5. Palavras encontradas e ausentes são exibidas.
6. O currículo é gerado sem informações inventadas.
7. Todo o currículo pode ser editado.
8. Copiar currículo funciona.
9. Exportar currículo gera PDF legível.
10. O design system pode ser visualizado e exportado.
11. O layout funciona em desktop e celular.
12. Não há botões principais sem função.
13. O app funciona sem backend ou chave de API.

## 16. Riscos e cuidados

- tratar estimativas como resultados garantidos;
- inserir palavras-chave de forma artificial;
- inventar experiência para aumentar a pontuação;
- gerar PDF visualmente bonito, mas ilegível por ATS;
- prometer inteligência artificial real sem integração implementada;
- expor dados pessoais do currículo.

## 17. Melhorias futuras

- autenticação opcional;
- histórico de vagas e versões;
- integração real com IA;
- importação de PDF ou DOCX;
- seleção de modelos de currículo;
- análise multilíngue;
- painel de candidaturas;
- testes com recrutadores e candidatos reais.