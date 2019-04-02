# o8-interview-fullstack

## Assignment

Create a simple to-do list application (shown on home screen) according to following specification:

### Functional criteria:

- I can see all to-dos with their status (complete/incomplete)
  - I can filter to-dos by complete/incomplete/all, defaults to 'All' (use custom buttons)
  - I can sort to-dos alphabetically
- I can complete/uncomplete a to-do

### Technical criteria:

- A to-do is a simple object having a numerical id, a message and a boolean indicator of whether or not it is completed.
- Create REST API (add TodosController) for the purposes of this assignment with following endpoints:
  - GET /todos
  - POST /todos
  - PUT /todos/{id}
  - DELETE /todos/{id}
- There is no need to save the data to a database, you can keep the data in memory
- Fetch the data from this API and store them in a Vuex module. Communicate with the API using Vuex actions, manage CRUD on the API and local state (filtering, sorting) in Vuex.
- Make sure you use separate components where appropriate, instead of creating one big component handling all of the logic. Reusability is key.
- If there are no to-dos to be shown, display a message saying so; when a button is unclickable (e.g. you can't undo an action of it is futher than 5 away), make it visually clear.
- Create a custom button for the purposes of the application, that you can display both with plain text and with an icon. Use Vue Slots to achieve this. Show use of Vue events to communicate with parent components.
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
