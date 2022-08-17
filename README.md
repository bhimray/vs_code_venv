# vs_code_venv

 Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted 


Operational Error

This occur because once you create a class (table) you have to do "makemigrations" followed by "migrate" if you don't then they will not find the table and won't be able to perform creating table from django admin page.

Fatal error in launcher: Unable to create process using '"C:\Users\Administrator\Desktop\env\Scripts\python.exe"  "C:\General_work\Django\djangoProj\env\Scripts\pip.exe" install djangorestframework': The system cannot find the file specified.
 so i installed pip as below:

python -m pip install --upgrade pip

after that i installed django rest framework



########################
Line 17:9:  Expected an assignment or function call and instead saw an expression  no-unused-expressions or eslint error
 then 
  return (
    <div>
      <h1>React Query Page</h1>
      {
      heroData.map((element)=>{
        console.log(element);
        <h1>{element.name}</h1> ###### here you have to keep return to return some value from function otherwise they will throw an error....
      })
      }
    </div>
  )
hence, 
the solution is
 return (
    <div>
      <h1>React Query Page</h1>
      {
      heroData.map((element)=>{
        console.log(element);
        return <h1>{element.name}</h1> #this will return html component while mapping through each data hence it works
      })
      }
    </div>
  )




parsing error: adjacent jsx elements must be wrapped in an enclosing tag. did you want a jsx fragment <>...</>?

while using map() function to loop ___
use <Fragement>
        <div> read this </div>
    </Fragement>


return some value from map function:
if there is nothing to return except to write the html then use
map(()=>(
)
otherwise use
map(()=>{
}

error in npm build in netlify

put CI= npm run build

This one will resolve the problems.



npm ERR! Could not resolve dependency:
npm ERR! peer react@"^16.8.0 || ^17.0.0" from @material-ui/core@4.12.4
npm ERR! node_modules/@material-ui/core
npm ERR!   @material-ui/core@"*" from the root project


then use npm install -f @material-ui/core
