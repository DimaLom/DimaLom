<div align="center">
  <code>Hello world!</code>
</div>
<br/>

<div align="center">
  <code><img height="30" alt="javascript" src="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg"></code>
  <code><img height="30" alt="typescript" src="https://github.com/devicons/devicon/blob/master/icons/typescript/typescript-original.svg"></code>
  <code><img height="30" alt="react" src="https://github.com/devicons/devicon/blob/master/icons/react/react-original.svg"></code>
  <code><img height="30" alt="nextjs" src="https://github.com/devicons/devicon/blob/master/icons/nextjs/nextjs-original.svg"></code>
  <code><img height="30" alt="vue" src="https://github.com/devicons/devicon/blob/master/icons/vuejs/vuejs-original.svg"></code>
  <code><img height="30" alt="redux" src="https://github.com/devicons/devicon/blob/master/icons/redux/redux-original.svg"></code>
  <code><img height="30" alt="sass" src="https://github.com/devicons/devicon/blob/master/icons/sass/sass-original.svg"></code>
  <code><img height="30" alt="graphql" src="https://github.com/devicons/devicon/blob/master/icons/graphql/graphql-plain.svg"></code>
  <code><img height="30" alt="nodejs" src="https://github.com/devicons/devicon/blob/master/icons/nodejs/nodejs-original.svg"></code>
  <code><img height="30" alt="express" src="https://github.com/devicons/devicon/blob/master/icons/express/express-original.svg"></code>
  <code><img height="30" alt="postgresql" src="https://github.com/devicons/devicon/blob/master/icons/postgresql/postgresql-original.svg"></code>
  <code><img height="30" alt="mongodb" src="https://github.com/devicons/devicon/blob/master/icons/mongodb/mongodb-original.svg"></code>
  <code><img height="30" alt="git" src="https://github.com/devicons/devicon/blob/master/icons/git/git-plain.svg"></code>
  <code><img height="30" alt="docker" src="https://github.com/devicons/devicon/blob/master/icons/docker/docker-original.svg"></code>
  <code><img height="30" alt="webpack" src="https://github.com/devicons/devicon/blob/master/icons/webpack/webpack-original.svg"></code>
  <code><img height="30" alt="figma" src="https://github.com/devicons/devicon/blob/master/icons/figma/figma-original.svg"></code>
</div>
<br/>

```JavaScript
class SoftwareEngineer {
    readonly name = 'Dmitriy'
    readonly lastName = 'Lomov'
    readonly birthdate = '12.07.1990'
    
    private technologies = {
        languages: [
            'JavaScript',
            'TypeScript'
        ],
        frontend: [
            'ReactJS',
            "NextJS",
            "VueJS",
            "GraphQL",
            'Redux',
            'RTK',
            'RTK Query',
            'MobX',
            'FSD',
            'Sass'
        ],
        backend: [
            'NodeJS',
            'Express',
            'NextJS'
        ],
        mobile: [
            'React Native',
            'Expo'
        ],
        UILibrary: [
            'MUI',
            'AntDesign',
            'NativeBase'
        ],
        dataBase: [
            'PostgreSQL',
            'MongoDB'
        ],
        other: [
            'git',
            'Docker',
            'Webpack',
            'Figma'
        ]
    }
    
    private calculateAge() {
        const day = parseInt(this.birthdate.substring(0, 2));
        const month = parseInt(this.birthdate.substring(3, 5));
        const year = parseInt(this.birthdate.substring(6, 10));
        
        const today = new Date();
        const birthDate = new Date(year, month - 1, day);
        const m = today.getMonth() - birthDate.getMonth();
        
        let age = today.getFullYear() - birthDate.getFullYear();
        
        if (m < 0 || (m === 0 && today.getDate() < birthDate.getDate())) {
            age--;
        }
        
        return age;
    }
    
    get fullName() {
        return `${this.lastName} ${this.name}`
    }
    
    get age() {
        return this.calculateAge()
    }
    
    public greetStranger() {
        return `
           Hello! My name is ${this.fullName}. I am ${this.age} years old. Glad to see you on my page.
           That's what I can: ${JSON.stringify(this.technologies, null, 4)}
        `
    }
}

const I = new SoftwareEngineer()

I.greetStranger()
```
