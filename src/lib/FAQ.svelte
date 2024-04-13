<script>
    let faqs = [
        { question: 'Question 1', answer: 'Answer 1' },
        { question: 'Question 2', answer: 'Answer 2' },
        // Add more FAQs as needed
    ];
    let openIndex = null;

    function toggleAnswer(index) {
        if (openIndex === index) {
            openIndex = null;
        } else {
            openIndex = index;
        }
    }
</script>

<style>
    .faq {
        width: 300px;
        border: 1px solid #000;
        padding: 10px;
        margin-bottom: 10px;
        cursor: pointer;
        background-color: #f9f9f9;
    }
    .answer {
        overflow: hidden;
        transition: max-height 0.2s ease-out;
        max-height: 0;
    }
    .answer.open {
        max-height: 100px;
    }
</style>

{#each faqs as { question, answer }, index}
    <div class="faq" on:click={() => toggleAnswer(index)}>
        {question}
        <div class="answer {openIndex === index ? 'open' : ''}">
            {answer}
        </div>
    </div>
{/each}
