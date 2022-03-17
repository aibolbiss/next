# Как установить NVM?
1) https://github.com/nvm-sh/nvm#install--update-script     -      ссылка для скачивания nvm
2) curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash     -     вставляем в терминал
3) export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm          -       вставляем в терминал
4) nvm --version
5) nvm install 12
6) node -v
7) nvm install 14
8) nvm use 14

# Как установить TypeScript?
1) npm install -g typescript
2) tsc --init      -      иницализируем tsconfig.json
3) создаем "index.ts", пишем код на "typescript" а потом в терминале пишем "tsc"

# Базовые типы
1) let a: number = 5;
2) let b: string = 'Aibol';
3) let c: boolean = true;
4) let d: string[] = ['Aibol', 'Zhanerke', 'Nurgul'];
5) let e: any = 7;

6) function test(a: string): number | string {
     return '';
   }
   
7) const test = (a: number): number => {
     return a * 2;
   }
   
8) d = d.map((item: string) => item.toUpperCase())     // ['AIBOL', 'ZHANERKE', 'NURGUL'];

9) function countCordination(cord:{lat: number, long?: number}){
   
   }
   
10) function test(id: number | string){
      if(typeof id === 'number'){
        console.log(id.toString());
      }
      else if(typeof id === 'string'){
        console.log(id.toUpperCase());
      }
    }
    
11) function test(a: number | number[]){
      if(Array.isArray(a)){
        // Проверка, является ли параметр "a" массивом?
      }
    }
    
    
# Interface and Type
1) interface IPoint{
     x: number,
     y: number
   }
   
   interface IPointTwo extends IPoint{
     z: number
   }
 
2) type Point = {
     x: number,
     y: number
   }
   
   type PointTwo = Point & {
     z: number
   }
   
3) interface ITest{
     a: number
   }
   
   interface ITest{
     b: number
   }
   
4) type Test = {
     a: number      // ошибка. В "Type" имплементация не работает
   }
   
   type Test = {
     b: number      // ошибка. В "Type" имплементация не работает
   }
    

# Литеральные типы
1) type actionType = 'up' | 'down'

   function performAction(action: actionType): -1 | 1 {
     switch(action){
       case 'down':
         return -1
       case 'up':
         return 1
     }
   }
     
   
   
