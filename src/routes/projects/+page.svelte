<script>
</script>

<svelte:head>
<title>Projects</title>
<meta name="description" content="Svelte demo app" />
</svelte:head>

<section >
<div class="w-full bg-[#2E2D3C] text-white h-20 text-3xl flex items-center pl-28">
    Projects
</div>
<div class="container mx-auto p-6">
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">

      <!-- Project 1: Personalized LLM -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden">
        <img src="llm.png" alt="Project 1" class="w-full h-48 object-cover">
        <div class="p-6">
            <h2 class="text-xl font-bold text-gray-800">Personalized LLM</h2>
            <p class="text-gray-600 mt-2">Get the LLM to give response based on the document of your choice. This application uses RAG approach, Langchain and Ollama to run model in your local machine.</p>
            <a href="https://github.com/0xmatriksh/local-llm" class="mt-4 inline-block text-[#2E2D3C] hover:underline">View Project</a>
          </div>
      </div>

      <!-- Project 2: Post Classification System -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden">
        <img src="flyer.png" alt="Post Classification System" class="w-full h-48 object-cover">
        <div class="p-6">
          <h2 class="text-xl font-bold text-gray-800">Post Classification System</h2>
          <p class="text-gray-600 mt-2">A website where people can read posts and discuss different categories of their interest easily. Classifies user’s post on some category using NLP and Machine Learning.</p>
          <a href="https://github.com/0xmatriksh/flyer" class="mt-4 inline-block text-[#2E2D3C] hover:underline">View Project</a>
        </div>
      </div>

      <!-- Project 3: Book Recommendation System -->
      <div class="bg-white rounded-lg shadow-lg overflow-hidden">
        <img src="books-recom1.png" alt="Book Recommendation System" class="w-full h-48 object-contain">
        <div class="p-6">
          <h2 class="text-xl font-bold text-gray-800">Book Recommendation System</h2>
          <p class="text-gray-600 mt-2">A website with collections of top-read books with the functionality of a recommendation system using Flask. Recommends books based on chosen books using Machine Learning.</p>
          <a href="https://github.com/0xmatriksh/Books-Recommendation-System/tree/master/Documents/DataScience/Books" class="mt-4 inline-block text-[#2E2D3C] hover:underline">View Project</a>
        </div>
      </div>

    </div>

</div>


</section>

<style>

</style>
