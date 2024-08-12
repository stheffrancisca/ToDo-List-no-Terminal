# ToDo-List-no-Terminal
ToDo List no Terminal


Crie um programa para criar uma lista de tarefas para o usuário (mais futuramente no curso, aprenderemos a armazenar essas informações em um banco de dados para essa lista poder ser editada e armazenada)

Seu programa deve pedir as tarefas que o usuário tem que fazer em um dia e, a cada inserção de uma nova tarefa, dizer que a tarefa foi adicionada a lista de tarefas. Quando o usuário digitar apenas enter no seu input (sem inserir nenhuma tarefa, seu programa deve printar a quantidade de tarefas para o dia e a lista de tarefas completa)

lista_tarefas = []

while True:
    tarefa = input("Escreva uma tarefa para adicionar a sua ToDo List")
    if tarefa == "":
        break
    else:
        lista_tarefas.append(tarefa)
        print(f"Tarefa adicionada com sucesso: {tarefa}")

print("Quantidade de tarefas para hoje:", len(lista_tarefas))
texto_tarefas = "\n".join(lista_tarefas)
print("Tarefas")
print(texto_tarefas)
