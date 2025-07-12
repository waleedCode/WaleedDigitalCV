<template>
  <section id="education" class="mb-16 scroll-mt-24">
    <h2 class="text-2xl font-bold text-blue-600 mb-10 text-center">Education</h2>

    <div class="relative border-l border-gray-300 pl-6 space-y-12">
      <div v-for="(edu, index) in education" :key="index" class="relative">
        <span class="absolute -left-1.5 top-2 w-3 h-3 bg-blue-600 rounded-full"></span>
        <div class="bg-white rounded-xl shadow-md border border-gray-200 p-6">
          <div class="flex justify-between flex-wrap mb-2">
            <h3 class="text-lg font-semibold text-gray-800">{{ edu.degree }}</h3>
            <span class="text-sm text-gray-400">{{ edu.date }}</span>
          </div>
          <p class="text-sm text-gray-500 mb-2">{{ edu.institution }}</p>
          <p class="text-sm text-gray-700">{{ edu.notes }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Education",
  data() {
    return {
      education: [
        {
          degree: "Master of Information Technology",
          institution: "Open University of Sudan — Khartoum, Sudan",
          date: "Expected Dec 2025",
          notes: "Currently in progress – one course remaining."
        },
        {
          degree: "Bachelor of Information Technology",
          institution: "Al-Neelain University — Khartoum, Sudan",
          date: "Dec 2020",
          notes: "Graduated with a strong foundation in web development and software engineering."
        },
      ]
    }
  }
}
</script>
