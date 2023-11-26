MONO REPO

packages/modules

REUSABLE CODE
Separation of concern - each module does what it is supposed to do
for eg: a file named day.js will contain everything related to days

ZOD infer

if in backend there if a type or interface introduced

// BACKEND
convert this zod object

const signInInput=z.object({
username:z.string(),
password:z.string(),
})

to this interface or type
//FRONTEND
interface input{
username:string,
password:string,

}

directly get values of zod object to the interface or type

type input=z.infer<typeof signInInput >
