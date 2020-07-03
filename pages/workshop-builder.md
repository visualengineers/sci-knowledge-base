---
layout: page
title: Workshop Builder
permalink: /workshop-builder
---

# Workshop Builder
The Workshop Builder **helps you plan and prepare workshops that fit your needs**. You may use it in advance of each workshop as the preliminary questions are always the same and the tips and tools are reusable. First of all, it is important to know the context and goal of the workshop. Next, the basic procedure can be determined and the appropriate knowledge items can be arranged. 

## Customize Your Workshop
Answer the following questions to get your personal Knowledge Item suggestions you can pick from. You will find workshop material and further instructions within each chosen Knowledge Item.

<div class="quizlist"></div>

<ol id="questions">
    <li>    
        <h3>Define your aim</h3>
        <p>Describe your goal as short and precise as possible. If you are stuck, perhaps the <a href="{{site.baseurl}}/terms/smart">S.M.A.R.T.</a> criteria or an “is not” analysis (excluding everything that is not the objective) will help.</p>   
        <!--<input type="textarea" id="aim" name="aim" size="100" placeholder="Type your aim here">-->
        <textarea id="a-1" rows="1" cols="100%" placeholder="Type your aim here!"></textarea>
    </li>
    <li>
        <h3>What's the number of participants?</h3>
        <input class="radio-option" type="radio" name="p" value="p-1" id="p-1" checked>
        <label class="for-radio-option" for="p-1"><i class="fas fa-users"></i>group</label>
        <input class="radio-option" type="radio" name="p" value="p-2" id="p-2">
        <label class="for-radio-option" for="p-2"><i class="fas fa-user"></i>individual</label>       
    </li>
    <li>   
        <h3>Where are you working from?</h3>
        <input class="radio-option" type="radio" name="l" value="l-1" id="l-1" checked>
        <label class="for-radio-option" for="l-1"><i class="fas fa-map-marker-alt"></i>same place</label>
        <input class="radio-option" type="radio" name="l" value="l-2" id="l-2">
        <label class="for-radio-option" for="l-2"><i class="fas fa-arrows-alt-h"></i>distributed</label>
    </li>
    <li>
        <h3> Choose a statement. I am / We are ...</h3>
        <input class="radio-text" type="radio" name="s" value="s-1" id="s-1">
        <label class="for-radio-text" for="s-1">at a certain development stage / interested in a certain topic.</label>
        <input class="radio-text" type="radio" name="s" value="s-2" id="s-2">
        <label class="for-radio-text" for="s-2">facing a complex challenge and don't know where to start.</label>
        <input class="radio-text" type="radio" name="s" value="s-3" id="s-3">
        <label class="for-radio-text" for="s-3">missing some theoretical background in design and implementation techniques.</label>
        <input class="radio-text" type="radio" name="s" value="s-4" id="s-4">
        <label class="for-radio-text" for="s-4">looking for practical knowledge within a specific research field / keyword.</label>
        <input class="radio-text" type="radio" name="s" value="s-5" id="s-5">
        <label class="for-radio-text" for="s-5">interested in everything or have multiple problems.</label>
        <button class="send" id="create-plan-btn">create plan</button>
    </li>
</ol>

<!-- BEGIN WORKSHOP PLAN-->
<div id="workshop-plan">

<h2>Your Workshop Plan</h2>


<div class="quizlist"></div>

<ol id="answers">
    <li>   
        <h3>Your Aim</h3>
        <div id="a-1-plan">
            <p class="answer"></p>
        </div>
        <div id="no-a-1-plan">
            <p class="answer">You didn't define an aim so far.</p>
            Have a look at the <a href="{{site.baseurl}}/terms/smart">S.M.A.R.T.</a> criteria or try doing an “is not” analysis (excluding everything that is not the objective). 
        </div>
    </li>
    <li>    
        <h3>Participants</h3>
        <div id="p-1-plan">
            <p class="answer">You are working in a team.</p>
        </div>
         <div id="p-2-plan">
            <p class="answer">Your are working on your own.</p>
        </div>
    </li>
    <li>  
        <h3>Workplace</h3>
        <div id="l-1-plan">
        <p class="answer">You are working at the same place.</p>
        These workshop tips for face-to-face collaboration might be helpful for you:
        interview Franzi, some concepts
        </div>
        <div id="l-2-plan">
        <p class="answer">You are working distributed.</p>
        These tools and concepts for remote collaboration could be helpful for you: 
        MIRO, some concepts
        </div>
    </li>
    <li> 
        <h3>Challenge</h3>
        <div id="s-1-plan"> 
            <p class="answer">You are at a certain development stage / interested in a certain topic.</p>
            We recommend a <b>thematic walktrough</b>. Search <a href="{{site.baseurl}}/best-practices">Best Practices</a> within a topic you are interested in and pick from the knowledge items.<br>
            <a class="topic topic-technology" href="{{site.baseurl}}/technology">technology</a>
            <a class="topic topic-ux" href="{{site.baseurl}}/ux">user experience</a>
            <a class="topic topic-design" href="{{site.baseurl}}/design">design</a> 
            <a class="topic topic-society" href="{{site.baseurl}}/society">society</a>.
        </div>
        <div id="s-2-plan">
        <p class="answer">You are facing a complex challenge and don't know where to start.</p>
        We recommend a <b>problem-oriented walktrough</b>. Search all <a href="{{site.baseurl}}/best-practices">Best Practices</a> and pick the knowledge items you are interested in.
        </div>
        <div id="s-3-plan">
        <p class="answer">You are missing some theoretical background in design and implementation techniques.</p>
        We recommend a <b>technology-oriented walktrough</b>. Search <a href="{{site.baseurl}}/terms-and-concepts/#concepts">concepts</a>.
        </div>
        <div id="s-4-plan">
        <p class="answer">You are looking for practical knowledge within a specific research field / keyword.</p>
        We recommend a <b>deep-dive approach</b>. Search by Keyword or browse <a href="{{site.baseurl}}/terms-and-concepts/#terms">terms</a>.<br><br>
        <input type="search" class="form-control td-search-input" placeholder=" Search this site…" aria-label="Search this site…" autocomplete="off">
        </div>
        <div id="s-5-plan">
       <p class="answer"> You are interested in everything or have multiple problems.</p>
        We recommend an <b>explorative walktrough</b>. Take a nap, start at the beginning of the page or let your cat browse SCI-KB.
        </div>
        <div id="no-s">
            <p class="answer">no answer</p>
        </div>
    </li>
</ol>

<button class="send" id="reset-btn">reset plan</button>

<!-- END WORKSHOP PLAN-->
</div>

<hr>
<br>
<p>Not sure if you want to hold a workshop? Have a look at our <a href="{{site.baseurl}}/10-questions-franziska">interview on holding workshops</a>.</p>

<script>

// short hand for $( document ).ready()
$(function() {
    
        // onload 
        $("#workshop-plan").hide();
        $('#questions').show();

        // create workshop plan
        $('#create-plan-btn').click(function () {

                let favourite = [];            
                $('#questions').hide();
                $("#workshop-plan").show();

                // textarea
                if (!$("#a-1").val().trim()) {
                     $('#a-1-plan').hide();
                     $('#no-a-1-plan').show();
                }
                else {
                    favourite.push($("#a-1").val());
                    let aim = $.trim($("#a-1").val());
                    $('#a-1-plan p').html(aim);
                    $('#a-1-plan').show();
                    $('#no-a-1-plan').hide();                    
                }                      
                
                $.each($("input:radio:not(:checked)"), function(){ 
                    $('#' + $(this).val() + '-plan').hide();
                });   

                if ($("input[name='s']:checked").val()) {
                     $('#no-s').hide();
                }            
       
        });

        // reset plan
        $('#reset-btn').click(function () {
            location.reload();
        });

});
</script>

  







