const express = require('express')
const app = express();


app.get('/alunos/:id', function (req, res) { 
    let alunos = ['Ana', 'João', 'Tales']
    let meuId = req.params.id
    return res.json ({
        nome: alunos[meuId] 
    })
})
    app.get('/alunos', (reg, res) => {
    res.json({qtd: 3, escola:'Ifcecrato'}); })

    app.get('/cursos', (reg,res) => {
res.json({qtd: 2, aulas: 8});
    })
app.listen(3000, () =>
{console.log('servidor rodando!')})

