produtos = []

while True:
    nome = input('adicione o produto: ' )
    data = input('adicione a data de validade: ' )
    preço = input('adicione o preço: ')
    produtos.append({'nome': nome, 'data': data, 'preço': preço})
    print(f'Produto: {nome}, Data de Validade: {data}, Preço: {preço}')
    print('produto adicionado com sucesso')
    print('quer adicionar mais produtos? (s/n)')
    resposta = input().lower()
    if resposta == 'n':
        break

print('\nLista de produtos adicionados:')
for produto in produtos:
    print(f"Produto: {produto['nome']}, Data de Validade: {produto['data']}, Preço: {produto['preço']}")


