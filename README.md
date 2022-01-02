# TP - Composants Vue.js

Votre objectif est de transformer ce CV en ligne en application Vue.js 

### Créez une application Vue.js grâce au CLI 
Suivez les indications données dans le cours
### Découpez l'application précédemment crée en composants réutilisables
Par exemple:
```html 
<SocialButton>
```
### Implémentez les Props dans tous vos composants 
Par exemple: 
```html 
<SocialButton url="https://twitter.com/MonCompte" icon="twitter">
```
### Gérez les données depuis Vue
Vos composants doivent devenir 100% dynamiques à cette étape. 
Vous gérerez une seule source de données, l'objet `data` de `App.vue`.

Par exemple: 

```javascript

export default {
  name: 'App',
  components: {
    Menu,
    ...
  },
  data: {
      socials: [
          {
              url: 'https://www.linkedin.com/in/maxence-machu/',
              icon: 'linkedin'
          }, 
          ...
      ],
      ...
  }
}
```
### Utilisez les directives
Servez-vous des directives comme `v-for` ou `v-if` pour gérer votre rendu de manière dynamique.
