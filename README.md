# Desafio — simulação educacional de ransomware

Material de estudo em **cibersegurança**: scripts em Python que ilustram, em ambiente controlado, o fluxo de um arquivo sendo criptografado com AES (modo CTR, via `pyaes`) e posteriormente restaurado. O propósito é **exclusivamente educacional** (laboratório, desafio acadêmico ou sandbox isolada).

**Não utilize estes scripts contra sistemas ou arquivos alheios.** Uso indevido é ilegal e antiético.

## Tecnologias

- Python 3
- Biblioteca `pyaes`

## Como executar

1. Crie um arquivo de teste chamado `teste.txt` na raiz do projeto (o `encrypter.py` lê esse nome fixo).

2. Instale a dependência:

```bash
pip install pyaes
```

3. Para simular a “infecção” (criptografia e remoção do original):

```bash
python encrypter.py
```

4. Para restaurar a partir do arquivo `.ransomwaretroll` gerado:

```bash
python decrypter.py
```

Os nomes de arquivo e a chave estão definidos no próprio código; adapte apenas para experimentos locais e nunca reutilize chaves fracas em produção.
