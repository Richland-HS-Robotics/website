    <style>
        .faq-question {
            cursor: pointer;
            padding: 10px;
            border: 1px solid #000;
            width: 300px;
            margin-bottom: 10px;
        }

        .faq-answer {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.2s ease-out;
            border: 1px solid #000;
            width: 300px;
            padding: 10px;
        }
    </style>
<div>    
    <div class="faq-question" onclick="document.getElementById('answer1').style.maxHeight = document.getElementById('answer1').style.maxHeight ? null : '100px'">
        Question 1
    </div>
    <div id="answer1" class="faq-answer">
        Answer 1
    </div>

    <div class="faq-question" onclick="document.getElementById('answer2').style.maxHeight = document.getElementById('answer2').style.maxHeight ? null : '100px'">
        Question 2
    </div>
    <div id="answer2" class="faq-answer">
        Answer 2
    </div>
</div>
