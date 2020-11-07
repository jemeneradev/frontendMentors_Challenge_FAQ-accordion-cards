<style>
  .Faq {
    position: relative;
    width: 327px;
    height: 535px;
    border-radius: 22px;
    /* background-color: red; */
    opacity: 0.5;
    background-color: white;

    margin: 0;
    margin-top: 140px;
    margin-left: 16px;
  }

  .Faq .Faq__graphic .Faq__graphic__foreground {
    position: relative;
    top: -108px;
    left: 16px;
  }

  .Faq .Faq__graphic .Faq__graphic__background {
    position: relative;
    top: -200px;
    left: 44px;
  }
  .Faq h1 {
    position: relative;
    top: -190px;
    left: 1px;
    text-align: center;
    /* FAQ */

    font-family: Kumbh Sans;
    font-style: normal;
    font-weight: bold;
    font-size: 32px;
    line-height: 32px;
    letter-spacing: 0.02em;
  }

  .Faq .Faq__questions {
    position: relative;
    top: -196px;
    width: 100%;
    height: 302px;
    margin: 0;
    padding: 0;
    /* background-color: red; */
    /* opacity: 0.3; */
  }

  .Faq .Faq__question {
    position: relative;
    width: 100%;
    height: 50px;
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .Faq__question h2 {
    font-family: Kumbh Sans;
    font-style: normal;
    font-weight: normal;
    font-size: 13px;
    line-height: 13px;
    margin: 0;
    margin-left: 25px;
    padding-top: 20px;
    /* identical to box height */

    color: #000000;
  }

  .Faq__question::after {
    content: url(images/icon-arrow-down.svg);
    display: block;
    width: fit-content;
    height: fit-content;
    position: absolute;
    top: 16px;
    left: 90%;
  }

  .Faq__question__answer {
    margin-left: 24px;
    width: 80%;

    font-family: Kumbh Sans;
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 18px;
    /* or 150% */

    color: #000000;

    display: none;
  }

  .Faq__question:hover {
    height: 98px;
    margin-bottom: 16px;
  }

  .Faq__question:hover h2 {
    font-weight: 700;
  }

  .Faq__question:hover::after {
    transform: rotate(180deg);
  }

  .Faq__question:hover .Faq__question__answer {
    display: block;
  }
  .Faq__question hr {
    position: relative;
    width: 85%;
    bottom: -9px;
  }
  .Faq__question:hover hr {
    bottom: -5px;
  }

  /*   .Faq .Faq__questions,
  .Faq__question {
    outline: solid 0.05rem black;
    opacity: 1;
  } */
</style>

<div class="Faq">
  <div class="Faq__graphic">
    <picture class="Faq__graphic__foreground">
      <source
        media="(min-width:1440px)"
        srcset="./images/illustration-woman-online-desktop.svg" />
      <source
        media="(max-width:1439px)"
        srcset="./images/illustration-woman-online-mobile.svg" />
      <img
        src="./images/illustration-woman-online-mobile.svg"
        alt="foreground: woman working on computer" />
    </picture>
    <picture class="Faq__graphic__background">
      <source
        media="(min-width:1440px)"
        srcset="./images/bg-pattern-desktop.svg" />
      <source
        media="(max-width:1439px)"
        srcset="./images/bg-pattern-mobile.svg" />
      <img
        src="./images/bg-pattern-mobile.svg"
        alt="background: woman working on computer icon shadow" />
    </picture>
  </div>
  <h1>FAQ</h1>
  <ul class="Faq__questions">
    <li class="Faq__question">
      <h2>How many team members can I invite?</h2>
      <div class="Faq__question__answer">
        <p>
          You can invite up to 2 additional users on the Free plan. There is no
          limit on team members for the Premium plan.
        </p>
      </div>
      <hr>
    </li>
    <li class="Faq__question">
      <h2>What is the maximum file upload size?</h2>
      <div class="Faq__question__answer">
        <p>
          No more than 2GB. All files in your account must fit your allotted
          storage space.
        </p>
      </div>
      <hr>
    </li>
    <li class="Faq__question">
      <h2>How do I reset my password?</h2>
      <div class="Faq__question__answer">
        <p>
          Click “Forgot password” from the login page or “Change password” from
          your profile page. A reset link will be emailed to you.
        </p>
      </div>
      <hr>
    </li>
    <li class="Faq__question">
      <h2>Can I cancel my subscription?</h2>
      <div class="Faq__question__answer">
        <p>
          Yes! Send us a message and we’ll process your request no questions
          asked.
        </p>
      </div>
      <hr>
    </li>
    <li class="Faq__question">
      <h2>Do you provide additional support?</h2>
      <div class="Faq__question__answer">
        <p>
          Chat and email support is available 24/7. Phone lines are open during
          normal business hours.
        </p>
      </div>
      <hr>
    </li>
  </ul>
</div>
