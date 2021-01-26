<template>
  <div>
    <h1>{{title}}</h1>
    <ul>
       <BookItem v-for="book in books" :book='book'></BookItem>
    </ul>
    <book-form @addBook='appendBook'></book-form>
      
    </div>
</template>

<script>
import BookItem from './BookItem';
import BookForm from './BookForm';
import BookForm from './BookForm.vue';
export default {
    components: {
    BookItem, BookForm
        BookForm,
  },
data () {
    return {
        title: "All Books",
        books: [
            {
            title: 'Self-Reliance', 
            author: 'Ralph Waldo Emerson'
            },
            {
            title: 'American Gods', 
            author: 'Neil Gaiman'
            },
            {
            title: 'Amusing Ourselves to Death',
            author: 'Neil Postman'},
]
    }
}
}
</script>

<style>
h1, h2 {
    font-weight: normal;
}
ul {
    list-style-type: none;
    padding: 0;
}

</style>