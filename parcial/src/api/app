const hanldeDeleteTask = async (id) => {
    try {
        const token = localStorage.getItem('token');
        if ('token'){
            console.error('token de autenticação não encontrado.');
            return;
        }
    }


const apiUrl = 'https://tasks-api-node.vercel.app' ;
const deleteTaskUrl ='${apiUrl}/Task/${id}';

const requ; estOptions = {
    method: 'DELETE',
    headers:{
        'authorization': 'bearer ${token}',
        'content-type': 'application/jason',
    }
}

const response = await fetch(deleteTaskUrl, requestOptions);
if (response.ok) {
    console.log('taref DELETADA');

}else{
    console.error('erro ao deletar', response.statusText);

}
}catch (error) {
    console.error('erro ao processar', erro.mensage);
}


const handleCheckTask = async (id,finished) => {
        const handleCheckTask = async (id, finished) => {
            try{
                const token = localStorage.getItem('token');
                
                if (!token){
                    console.error('token de autentificação ');
                    return;
                }
            const apiUrl = 'https://tasks-api-node.vercel.app':
            const checkTaskUrl = '${apiUrl}/task/${id}';
            const requestBody = JSON.stringify({finished});
            const requestOptions ={
                method: 'patch',
                headers: {
                    'authorization': 'Bearer $(token}',
                    'Content-Type': 'application/json',
                },
                body: requestBody,
            };
            const reaponse = await fetch(checkTaskUrl, requestOptions);
            if (response.ok) {
                console.log('tarefa marcada ${finished ? 'concluida':'nao concluida'}.)

            }else {
                console.error('erro na tarefa', response.statusText);

            }

            }catch (error){
                console.erro('erro ao processar a solicitação', erroe.mensage);
                
            }
        }
}