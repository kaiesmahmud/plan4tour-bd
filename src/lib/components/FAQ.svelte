<script >
    import * as Accordion from "$lib/components/ui/accordion";
    let data = [
      {
        id:'01',
        question: "Best time to visit Cox's Bazar?",
        answer: "The best time to visit Cox's Bazar is during the dry season, which runs from November to March. The weather is pleasant during this time, with plenty of sunshine and little rain. However, Cox's Bazar can be crowded during this time, so it is advisable to book your accommodation in advance.",
      },
      {
        id: "02",
        question: "Best things to do in Cox's Bazar?",
        answer: "There are many things to do in Cox's Bazar, including swimming, sunbathing, surfing, and fishing. You can also visit the nearby St. Martin's Island, which is a popular spot for snorkeling and diving.",
      },
      {
        id: "03",
        question: "How can I get to Cox's Bazar?",
        answer: "Cox's Bazar is located in the southeastern part of Bangladesh. The nearest airport is Cox's Bazar Airport (CXB), which is served by domestic flights from Dhaka and Chittagong. You can also take a train or bus from Dhaka or Chittagong.",
      },
      {
        id: "04",
        question: "Where can I stay in Cox's Bazar?",
        answer: "There are many hotels and resorts in Cox's Bazar, to suit all budgets. Some of the most popular hotels include the Sea Shell Hotel, the Le Meridien Hotel, and the Long Beach Hotel.",
      },
      {
        id: "05",
        question: "How much does it cost to travel to Cox's Bazar?",
        answer: "The cost of travel to Cox's Bazar will vary depending on your budget and travel style. However, as a general rule of thumb, you can expect to spend around US$100-200 per day on accommodation, food, and activities.",
      },
    ]
  </script>
  <div class="flex items-center justify-center p-3 relative">
    <div class='absolute w-[200px] h-[200px] md:w-[400px] md:h-[400px] gradient-04 opacity-20 md:opacity-30 top-[-200px] left-0 gradient-animation' />

    <div class="w-full md:w-[80%] p-5 rounded shadow bg-white/10">
      <h1 class="text-center pb-5">Frequently Asked Questions or Enquires </h1>
      <Accordion.Root >
        {#each data as item}
          <Accordion.Item value={item.id}>
            <Accordion.Trigger>{item.question}</Accordion.Trigger>
            <Accordion.Content>{item.answer}</Accordion.Content>
          </Accordion.Item>
        {/each}
      </Accordion.Root>
    </div>
  </div>
  
