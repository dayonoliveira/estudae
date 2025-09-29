# Especificações da API

## Cadastro

### Criar usuário

- URI: `/register`
- Método: POST
- Request Body:
```json
{ "name": "", "email": "", "birthdate": "", "password": "" }
```

### Definir perfil Estudante

- URI: `/register/user-role/student`
- Método: POST
- Request Body:
```json
{ "educationLevel": "", "grade": "", "studentSubjects": [] }
```

### Definir perfil Mentor

- URI: `/register/user-role/mentor`
- Método: POST
- Request Body:
```json
{ "firstSubject": "", "secondSubject": "", "thirdSubject": "" }
```

### Definir perfil Voluntário

- URI: `/register/user-role/volunteer`
- Método: POST
- Request Body:
```json
{ "donatingThing": "" }
```

## Login

### Autenticação

- URI: `/login`
- Método: POST
- Request Body:
```json
{ "email": "", "password": "" }
```

## Solicitações

### Estudantes

#### Listar minhas solicitações

- URI: `/my-requests`
- Método: POST
- Request Body:
```json
{ "page": 0, "size": 10 }
```

#### Obter solicitação por ID

- URI: `/my-requests/{requestId}`
- Método: GET
- Path Param: `requestId` (number)

#### Criar solicitação

- URI: `/requests`
- Método: POST
- Request Body:
```json
{ "requestType": "", "title": "", "description": "" }
```

#### Atualizar solicitação

- URI: `/requests`
- Método: PATCH
- Request Body:
```json
{ "requestType": "", "title": "", "description": "" }
```

#### Excluir solicitação

- URI: `/requests/{requestId}`
- Método: DELETE
- Path Parameter: requestId (number)

### Mentores e Voluntários

#### Listar solicitações de estudantes disponíveis

- URI: `/available-student-requests`
- Método: POST
- Request Body:
```json
{ "page": 0, "size": 10 }
```

#### Obter solicitação de estudante por ID

- URI: `/available-student-requests/{requestId}`
- Método: GET
- Path Param: requestId (number)

#### Aceitar solicitação de estudante

- URI: `/accept-student-requests`
- Método: POST
- Request Body:
```json
{ "requestId": "", "studentId": "" }
```

#### Finalizar solicitação de estudante

- URI: `/finish-student-requests`
- Método: PATCH
- Request Body:
```json
{ "requestId": "", "studentId": "" }
```

#### Cancelar solicitação de estudante

- URI: `/cancel-student-requests/{requestId}`
- Método: DELETE
- Path Param: requestId (number)
