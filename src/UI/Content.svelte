<section class="content">
  <img src="../images/image-web-3-desktop.jpg" alt="desktop" />
  <article class="right-grid">
    <h2>New</h2>
    <p class="sub-header">Hydrogen VS Electric Cars</p>
    <p>Will hydrogen-fueled cars ever catch up to EVs?</p>
    <p class="sub-header">The Downsides of AI Artistry</p>
    <p>
      What are the possible adverse effects of on-demand AI image generation?
    </p>
    <p class="sub-header">Is VC Funding Drying Up?</p>
    <p>
      Private funding by VC firms is down 50% YOY. We take a look at what that
      means.
    </p>
  </article>
  <h1 class="bold-header">The Bright <br /> Future of Web <br /> 3.0?</h1>
  <article class="bar">
    <p class="light-header">
      We dive into the next evolution of the web that claims to put the power of
      the platforms back into the hands of the people. But is it really
      fulfilling its promise?
    </p>
    <span class="btn">Read more</span>
  </article>
</section>

<style>
  .content {
    width: 100%;
    display: grid;
    gap: 0.3rem;
    grid-template-areas:
      "head head bar"
      "nav main bar";
    grid-template-columns: repeat(3, 33%);
    /* grid-template-rows: repeat(2, 0.4fr); */
    padding-top: 0.5rem;
  }
  .content img {
    width: 97%;
    height: 90%;
    grid-area: head;
  }
  .right-grid {
    grid-area: bar;
    padding: 0.5rem 1rem;
    background-color: hsl(240, 100%, 5%);
    color: hsl(36, 100%, 99%);
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
  }
  .right-grid h2 {
    color: hsl(35, 77%, 62%);
    font-weight: bold;
    padding-top: 1rem;
  }
  .right-grid .sub-header {
    font-weight: bold;
    padding: 1.6rem 0rem 0 0;
  }
  .right-grid > p:not(.sub-header) {
    opacity: 0.6;
  }

  .bold-header {
    grid-area: nav;
  }
  .bar {
    grid-area: main;
    margin-right: 2rem;
  }
  .sub-header {
    margin: 0.2rem 0 0.5rem 0;
    padding: 0.6rem 0 0.5rem 0;
  }
  .bold-header {
    font-size: 2rem;
    font-weight: bolder;
    padding: 0 2rem;
    margin-top: 0;
    margin-bottom: 0;
  }
  .btn {
    background: red;
    display: block;
    margin-top: 0.5rem;
    padding: 0.3rem 0.5rem 0.3rem 0.5rem;
    width: 120px;
  }
  @media (max-width: 1180px) {
    .right-grid h2 {
      font-size: 1rem;
    }
    .right-grid > p:not(.sub-header) {
      font-size: 0.8rem;
    }
  }
  @media (max-width: 1018px) {
    .right-grid h2 {
      font-size: 0.8rem;
      padding-top: 0.5rem;
    }
    .right-grid > p:not(.sub-header) {
      font-size: 0.6rem;
      margin: 0;
      padding: 0 0.2rem;
    }

    .sub-header {
      padding: 0;
      font-size: 1.12rem;
    }
  }

  @media (max-width: 698px) {
    .content {
      display: flex;
      flex-direction: column;
      padding: 0 0.5rem;
      margin-bottom: 5rem;
    }
    .content img {
      padding: 1rem 0;
      margin-left: 0rem;
      height: 350px;
      width: 100%;
    }
    h1.bold-header {
      order: 2;
      height: 17%;
      text-align: start;
      padding-left: 0;
      width: 60%;
      /* margin-left: 0.5rem; */
    }
    .bar {
      order: 3;
      height: 30%;
      padding: 0.7rem 0;
      /* margin-left: 0.5rem; */
      width: 100%;
      font-size: 1.2rem;
    }
    .btn {
      margin-top: 1rem;
      background: hsl(5, 85%, 63%);
      color: hsl(36, 100%, 99%);
      padding: 0.7rem 1rem 0.7rem 0.5rem;
      width: 34%;
      border-radius: 2px;
      display: flex;
      align-items: center;
      justify-content: center;
      line-height: 10px;
      cursor: pointer;
      margin-bottom: 2rem;
    }
    .right-grid {
      order: 4;
      padding: 0.5rem;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding-left: 3rem;
      /* word-spacing: px; */
      letter-spacing: 2px;
      margin-bottom: 4.5rem;
    }
    .right-grid h2 {
      margin: 0rem;
      padding: 0.5rem 0 0.5rem 1rem;
      font-size: 2.3rem;
    }
    .right-grid .sub-header {
      margin: 0;
      padding: 0.5rem 0 0.5rem 1rem;
      font-size: 1.3rem;
    }
    .right-grid > p:not(.sub-header) {
      font-size: 16px;
      padding: 0.5rem 0 1rem 1rem;
      width: 69%;
    }
    .right-grid p:nth-of-type(2),
    .right-grid p:last-of-type {
      border-bottom: 1px solid hsl(36, 100%, 99%);
      padding-right: 1rem;
      width: 76%;
    }
  }
</style>
