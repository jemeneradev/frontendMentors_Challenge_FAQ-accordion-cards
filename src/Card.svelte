<style>
  /*  .Faq__info {
    outline: solid 1px black;
  }
  .Faq__info .Faq__questions{
    outline: solid 1px green;
  }
  .Faq__info .Faq__questions .Faq__question{
    outline: solid 1px orange;
  } */

  .Faq {
    position: relative;
    width: 100%;
    height: 535px;
    border-radius: 22px;
    /* background-color: red; */
    /* opacity: 0.5; */
    background-color: white;

    margin: 0;
    top: -35px;
    left: 16px;
    filter: url("#CardShadow");
  }

  .Faq__graphic .Faq__graphic__foreground {
    position: relative;
    top: -108px;
    left: -15px;
  }

  .Faq__graphic .Faq__graphic__background {
    position: relative;
    top: -203px;
    left: 0px;
  }

  .Faq__graphic__box {
    display: none;
  }

  .Faq__info {
    position: relative;
    top: -197px;
  }

  .Faq__info h1 {
    position: relative;
    text-align: center;
    /* FAQ */

    font-family: Kumbh Sans;
    font-style: normal;
    font-weight: bold;
    font-size: 32px;
    line-height: 32px;
    letter-spacing: -0.005em;
  }

  .Faq__info .Faq__questions {
    position: relative;
    width: 100%;
    height: 302px;
    margin: 0;
    padding: 0;
    /* padding-top: 18px;
    top: -6px; */
    /* background-color: red; */
    /* opacity: 0.3; */
  }

  .Faq__question {
    box-sizing: content-box;
    position: relative;
    width: 100%;
    height: 32px;
    margin: 0;
    padding: 0;
    list-style: none;
    padding-top: 13px;
    margin-bottom: 7px;
  }

  .Faq__question h2 {
    font-family: Kumbh Sans;
    font-style: normal;
    font-weight: normal;
    font-size: 13px;
    line-height: 13px;
    margin: 0;
    margin-left: 25px;
    text-align: left;
    /* identical to box height */

    color: #000000;
  }

  .Faq__question::after {
    content: url(images/icon-arrow-down.svg);
    display: block;
    width: fit-content;
    height: fit-content;
    position: absolute;
    top: 5px;
    left: 90%;
  }

  .Faq__question__answer {
    width: 80%;
    display: none;

    margin: 0;
    margin-left: 24px;
    margin-top: 13px;
  }

  .Faq__question__answer > p {
    font-family: Kumbh Sans;
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 18px;
    /* or 150% */

    color: #000000;
    text-align: left;
    margin: 0;
  }

  .Faq__question:hover {
    height: 76px;
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
    position: absolute;
    width: 85%;
    bottom: 0px;
    margin: 0;
    margin-left: 25px;
    /* margin-top: 18px; */
  }
  .Faq__question:hover hr {
    bottom: -5px;
  }

  @media screen and (min-width: 1440px) {
    .Faq {
      /* 
      margin: auto 273px; */
      width: 920px;
      height: 509px;

      display: flex;
      top: -159px;
      left: 273px;
    }

    .Faq__graphic {
      overflow-y: hidden;
      width: 45%;
      position: relative;
    }

    .Faq__graphic .Faq__graphic__foreground {
      top: 70px;
      left: -84px;
      z-index: 1;
    }

    .Faq__graphic .Faq__graphic__background {
      top: -661px;
      left: -578px;
      /* overflow: hidden; */
      z-index: 0;
    }

    .Faq__graphic__box {
      display: block;
      position: absolute;
      top: 204px;
      left: -93px;
      height: fit-content;
      width: fit-content;
      overflow-x: visible;
      z-index: 2;
    }
    .Faq__info {
      position: relative;
      left: 37px;
      top: 245px;
      width: 44%;
    }

    .Faq__info h1 {
      text-align: left;
      top: -195px;
      left: 24px;
    }

    .Faq__questions {
      top: -189px;
    }

    .Faq__question__answer {
      font-size: 14px;
    }

    .Faq__question h2 {
      letter-spacing: 0.042em;
    }

    .Faq__question::after {
      left: 87%;
    }
  }
  /*   .Faq .Faq__questions,
  .Faq__question {
    outline: solid 0.05rem black;
    opacity: 1;
  } */
</style>
<svg>
  <filter id="CardShadow">
    <feMorphology in="SourceGraphic" operator="dilate" radius="2"/>
    <feGaussianBlur stdDeviation="15" result="BLURED_FIGURE"/>
    <feOffset in="BLURED_FIGURE" dy="15" result="OFFSET"/>
    <feBlend in="SourceGraphic" in2="OFFSET" mode="normal" result="SHADOW"/>
    <feFlood flood-color="black" flood-opacity=".3" result="flood"/>
    <feComposite in="flood" in2="SHADOW" operator="in" result="DROPSHADOW"/>
    <feMerge>
      <feMergeNode in="DROPSHADOW"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>
</svg>

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
  <picture class="Faq__graphic__box">
    <source
      media="(min-width:1440px)"
      srcset="./images/illustration-box-desktop.svg" />
    <img
      src="./images/illustration-box-desktop.svg"
      alt="background: woman working on computer icon shadow" />
  </picture>
  <div class="Faq__info">
    <h1>FAQ</h1>
    <ul class="Faq__questions">
      <li class="Faq__question">
        <h2>How many team members can I invite?</h2>
        <div class="Faq__question__answer">
          <p>
            You can invite up to 2 additional users on the Free plan. There is
            no limit on team members for the Premium plan.
          </p>
        </div>
        <hr />
      </li>
      <li class="Faq__question">
        <h2>What is the maximum file upload size?</h2>
        <div class="Faq__question__answer">
          <p>
            No more than 2GB. All files in your account must fit your allotted
            storage space.
          </p>
        </div>
        <hr />
      </li>
      <li class="Faq__question">
        <h2>How do I reset my password?</h2>
        <div class="Faq__question__answer">
          <p>
            Click “Forgot password” from the login page or “Change password”
            from your profile page. A reset link will be emailed to you.
          </p>
        </div>
        <hr />
      </li>
      <li class="Faq__question">
        <h2>Can I cancel my subscription?</h2>
        <div class="Faq__question__answer">
          <p>
            Yes! Send us a message and we’ll process your request no questions
            asked.
          </p>
        </div>
        <hr />
      </li>
      <li class="Faq__question">
        <h2>Do you provide additional support?</h2>
        <div class="Faq__question__answer">
          <p>
            Chat and email support is available 24/7. Phone lines are open
            during normal business hours.
          </p>
        </div>
        <hr />
      </li>
    </ul>
  </div>
</div>
