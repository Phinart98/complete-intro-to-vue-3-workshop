<script>
export default {
  data() {
    return {
      characters: [
        'Jon Snow',
        'Arya Stark',
        'Cersei Lannister',
        'Jamie Lanister',
        'Sansa Stark',
        'Ned Stark'
      ],
      emptyCharacters: [],
      employees: ['Christian', 'Amdy', 'Danny', 'Gloria', 'Enoch', 'Philip']
    }
  }
}
</script>

<template>
  <div>
    <table>
      <thead>
        <tr>
          <th>GoT Characters</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="c in characters">
          <td>{{ c }}</td>
        </tr>
        <tr v-for="e in employees">
          <td>{{ e }}</td>
        </tr>
      </tbody>
    </table>
    <!-- <ul v-if="emptyCharacters.length !== 0">
        <li v-else>Charater List is Empty</li>
        <li v-for="c in emptyCharacters>{{ c }}</li>
      </ul> -->
  </div>
</template>

<style scoped></style>
