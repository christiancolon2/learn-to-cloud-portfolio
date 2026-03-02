# Week 01 — Hello Azure (Azure CLI Proof)

## Goal

Prove I can authenticate and manage Azure resources using the Azure CLI.

---

## 1) Azure CLI Installed

**Command:**

```bash
az version
```

[Azure Version](Link Here)

```bash
az login
```

```bash
az account show
```

[Account Show](Link Here)

```bash
az account list --output table
```

**If you have more than one subscription, set the one you want:**

```bash
az account set --subscription "SUBSCRIPTION_NAME_OR_ID"
```

**Create a Resource Group(CLI)**

- Resource group: rg-week01-hello-azure
- Location: eastus (or whatever region you prefer)

```bash
az group create --name rg-week01-hello-azure --location eastus
```

[Resource Group Created](Link Here)

```bash
az group list --output table
```

[Resource Group table](Link Here)

```bash
az group show --name rg-week01-hello-azure
```

## 6) Delete IT (CLI) - Cleanup Proof

```bash
az group delete --name rg-week01-hello-azure --yes --no-wait
```

**Confirm It's Gone**

```bash
az group exists --name rg-week01-hello-azure
```
