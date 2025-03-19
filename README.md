# Como consertar o "error: remote origin already exists"

## O erro "remote origin already exists" significa que o repositório remoto já foi configurado anteriormente. Para corrigir isso, você deve fazer o seguinte:

## Verificar a origin

### Para verificar o local da origin digite:
```
git remote -v
```
#### Isso mostrará algo assim:
```
origin  https://github.com/seu-usuario/seu-repositorio.git (fetch)
origin  https://github.com/seu-usuario/seu-repositorio.git (push)
```
#### Se o link do repositório for estiver correto e for o mesmo do seu repositório, é só continuar digitando:
```
git push -u origin main
```
#### Após isso o repositório estará sincronizado com o GitHub

## Substituir o remote existente

### Se o remote estiver errado ou precisar ser atualizado, remova-o e adicione novamente:
```
git remote remove origin
```
```
git remote add origin https://github.com/seu-usuario/seu-repositorio.git
```
#### Lembre-se de colar a URL do seu repositório
```
git push -u origin main
```

## Assim a sua origin será atualizada para o repositório atual e você poderá enviar o seu código para o GitHub normalmente!

### Para saber como enviar seu código do VS Code para o GitHub acesse meu outro repositório:
### [Enviando-codigo-do-VS-Code-para-repositorio-no-GitHub](https://github.com/Enzo-Camelo/Enviando-codigo-do-VS-Code-para-repositorio-no-GitHub)
