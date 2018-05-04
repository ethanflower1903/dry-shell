# Don't repeat yourself (DRY)

Adicione a biblioteca no seu projeto

```
git submodule add ssh://git@gitlab.f13.com.br:7222/sysadmin/fun-shell.git fslib
```

Exemplos 

```bash
source ${PWD}/enviroment/index.sh
source ${PWD}/input/index.sh
source ${PWD}/os/index.sh
source ${PWD}/is/index.sh

export userInput='teste AUTOMATIZADO'
input
#enviroment.debug
if [[ `input.inverse` == 'TESTE automatizado' ]];then 
    echo 'Input inverse it`s work!'
fi

#enviroment.debug
if ! os.file.path read "/root"; then
    echo 'Path read permisiso it`s work!'
fi

#enviroment.debug
if ! is.ip.v4 113.213.1s3.13 ;then
    echo 'Ip v4 test it`s work!'
fi
```