# o8-interview-fullstack

## Assignment

Create a simple to-do list application (shown on home screen) according to following specification:

### Functional criteria:

- I can see all to-dos with their status (complete/incomplete)
  - I can filter to-dos by complete/incomplete/all, defaults to 'All'
  - I can sort to-dos alphabetically in ascendent or descendent manner
- I can complete/uncomplete a to-do
- If there are no to-dos to be shown, display a message saying so

### Technical criteria:

- A to-do is a simple object having a numerical id, a message and a boolean flag indicating its completion.
- Create REST API (add TodosControlelr) with following endpoints:
  - GET /todos
  - PUT /todos/{id}
  - There is no need to save the data into a database, you can keep it in memory
- Fetch the data from the API and store it in a Vuex module. Interact with the API using Vuex actions mapped to the endpoints, and manage local state (filtering, sorting) in Vuex.
- Make sure you use separate components where appropriate, instead of creating one big component handling all of the logic. Reusability is key.
- If there are no to-dos to be shown, display a message saying so; when a button is unclickable (e.g. you can't undo an action of it is futher than 5 away), make it visually clear.
- Create a custom button for the purpose of filtering, sorting, completing and uncompleting todos.
  - Enable the display of any content (plain text, icon) injected from outside the component, use Vue slots to achieve this.
  - Distinguish the buttons with icons, feel free to use any publicly avaiable on the internet.
- Show use of Vue events to communicate with parent components
- (Optional) Style the component according to your own taste, preferably using SASS (style lang="scss" in .vue files) and adhering to BEM methodology. Do not spend too much time on this point as it is not too important for the completion of the assignment.

## Useful reading

- [TypeScript documentation](http://typescriptlang.com/)
- [vue-class-component documentation](https://github.com/vuejs/vue-class-component)
- [vue-property-decorator documentation](https://github.com/kaorun343/vue-property-decorator)
- [vuex-class documentation](https://github.com/ktsn/vuex-class)

## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```

### Compiles and minifies for production

```
npm run build
```

### Run your tests

```
npm run test
```

### Lints and fixes files

```
npm run lint
```

### Run your unit tests

```
npm run test:unit
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).
