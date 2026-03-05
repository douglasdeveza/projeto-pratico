# 🚀 Pipeline CI/CD Multi-OS com Integração SonarCloud

[![Missao 2 — CI Multi-OS + Segurança (Sonar)](https://github.com/douglasdeveza/multi-os-ci-pipeline-sonar/actions/workflows/missao2-sonarqube.yml/badge.svg)](https://github.com/douglasdeveza/multi-os-ci-pipeline-sonar/actions/workflows/missao2-sonarqube.yml)

## 📌 Sobre o Projeto

Este projeto demonstra a implementação de uma pipeline de Integração Contínua (CI) utilizando GitHub Actions com execução em múltiplos sistemas operacionais (Windows e Linux), evoluindo posteriormente para integração com análise estática de código via SonarCloud.

O objetivo foi aplicar, de forma prática, conceitos de CI/CD, automação e DevSecOps em ambiente controlado.

---

## 📈 Evolução do Projeto

O desenvolvimento ocorreu em duas etapas:

**Fase 1 – Pipeline Multi-OS**
- Execução de jobs em Windows e Linux
- Estruturação de workflow com múltiplos runners
- Disparo automático via push e pull request

**Fase 2 – Integração DevSecOps**
- Integração com SonarCloud para análise estática
- Execução do SonarScanner via CLI no Windows
- Execução via Action oficial no Linux
- Uso de secrets para autenticação segura
- Implementação de cache para otimização da pipeline

---

## 🧱 Arquitetura da Pipeline

O workflow é composto por quatro jobs independentes:

1. Hello World - Windows  
2. Hello World - Linux  
3. Sonar Scan - Windows (via CLI manual)  
4. Sonar Scan - Linux (via Action oficial)  

A pipeline é acionada em:

- Push na branch `main`
- Pull Requests
- Execução manual (`workflow_dispatch`)

---

## 🔐 Segurança

- Utilização de `SONAR_TOKEN` armazenado como secret no GitHub
- Integração com SonarCloud para análise de qualidade de código
- Estrutura preparada para aplicação de Quality Gate
- Aplicação prática de conceitos de DevSecOps

---

## ⚙️ Tecnologias Utilizadas

- GitHub Actions
- YAML
- SonarCloud
- Java (Temurin 17)
- Multi-OS Runners (Windows & Ubuntu)
- Conceitos de DevSecOps

---

## 🎯 Conceitos Aplicados

- Integração Contínua (CI)
- Automação de pipeline
- Execução paralela de jobs
- Setup manual de ferramentas em runner Windows
- Uso de cache para otimização
- Gerenciamento seguro de credenciais
- Integração com ferramenta de análise estática

---

## 📚 Objetivo Técnico

Consolidar conhecimentos práticos em CI/CD e DevSecOps, estruturando pipelines multi-ambiente com integração de ferramentas de segurança amplamente utilizadas no mercado.

---

Projeto desenvolvido para prática e aprimoramento técnico em DevOps.
