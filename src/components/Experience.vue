<template>
  <section id="experience" class="mb-16 scroll-mt-24">
    <h2 class="text-2xl font-bold text-blue-600 mb-10 text-center">Professional Experience</h2>

    <div class="relative border-l border-gray-300 pl-6 space-y-12">

      <!-- Timeline Entry -->
      <div v-for="(job, index) in jobs" :key="index" class="relative">
        <span class="absolute -left-1.5 top-2 w-3 h-3 bg-blue-600 rounded-full"></span>
        <div class="bg-white rounded-xl shadow-md border border-gray-200 p-6">
          <div class="flex justify-between flex-wrap mb-2">
            <h3 class="text-lg font-semibold text-gray-800">{{ job.title }}</h3>
            <span class="text-sm text-gray-400">{{ job.date }}</span>
          </div>
          <p class="text-sm text-gray-500 mb-3">{{ job.company }}</p>
          <ul class="list-disc list-inside text-sm text-gray-700 space-y-1">
            <li v-for="(point, i) in job.details" :key="i">{{ point }}</li>
          </ul>
        </div>
      </div>

    </div>
  </section>
</template>

<script>
export default {
  name: "Experience",
  data() {
    return {
      jobs: [
        {
          title: "Full Stack Developer",
          company: "Emdadat Alatta — Riyadh, Saudi Arabia",
          date: "Oct 2024 – Present",
          details: [
            "Developed scalable APIs and backend logic for ERP systems using Laravel",
            "Enhanced inventory and finance modules and supported multiple active business apps",
            "Optimized performance and integrated secure data practices",
            "Connected external third-party tools and services",
          ],
        },
        {
          title: "Backend Developer",
          company: "Mask Information Technology Company — Jeddah, Saudi Arabia",
          date: "Mar 2024 – Sep 2024",
          details: [
            "Built and maintained Laravel-based RESTful APIs for business applications",
            "Collaborated with frontend and operations teams in a hybrid work environment",
            "Created reusable components and optimized database performance",
          ],
        },
        {
          title: "Software Engineering Manager",
          company: "Online Auction — Jeddah, Saudi Arabia",
          date: "Mar 2022 – Feb 2024",
          details: [
            "Directed backend development for logistics platforms (mobile & client portals)",
            "Managed sprints with Jira, collaborated with stakeholders and product teams",
            "Oversaw CI/CD pipelines, DevOps, and source control practices",
            "Integrated analytics, marketing features, and third-party APIs",
            "Analyzed requirement documents to deliver business-specific solutions",
            "Led standups, sprint planning, architecture reviews, and hiring evaluations",
            "Improved software quality through engineering standards and team mentorship",
          ],
        },
        {
          title: "Teaching Assistant",
          company: "Al-Neelain University (Faculty of CS & IT) — Khartoum, Sudan",
          date: "Nov 2021 – Mar 2022",
          details: [
            "Assisted in teaching programming, web development, and database courses",
            "Led hands-on labs in PHP, HTML5, CSS, and JavaScript",
            "Helped design course materials and supported student projects",
          ],
        },
        {
          title: "Full Stack Developer (Contract)",
          company: "UNESCO — Khartoum, Sudan",
          date: "Jan 2020 – May 2021",
          details: [
            "Built a full-stack news publishing platform with admin role control",
            "Developed Laravel backend and Bootstrap/jQuery frontend",
            "Implemented multilingual support and cloud deployment",
            "Designed MySQL schemas and offered end-user technical support",
          ],
        },
      ],
    };
  },
};
</script>
