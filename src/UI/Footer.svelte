
<style>
    .footer{
        display: flex;
        text-align: center;
        height: 135px;
        margin-top: 1rem;
    }
    img{
        height: auto;
    }
    .item-one,.item-two,.item-three{
        display: flex;
        width: 100%;
        justify-content: space-between;
    }
    .num{
        margin-left: 0;
        text-align: start;
        padding: 0 0.5rem;
        opacity: 0.6;
    }
    .num-par{
        text-align: start;
        padding: 0 0.5rem;
        font-weight: bolder;
    }
    .num-detail{
        text-align: start;
        padding: 0  0.5rem;
    }
    .footer-content{
        display:flex;
        flex-direction: column;
        justify-content: space-around;
    }

    @media (max-width: 956px){
        .num{
            font-size: 20px;
        }
        .num-detail{
            font-size: 13px;
        }
    }
    @media(max-width: 698px){
      .footer{
        display: flex;
        flex-direction: column;
        height: 600px;
        justify-content: center;
        align-items: center;
        margin-top: 0;
      }
      
      .item-one,.item-two, .item-three{
        display: flex;
        align-items: center;
        padding: 0.5rem 0rem;
        width: 92% !important;
        justify-content: center;
      }
      .item-one img, .item-two img, .item-three img{
        height: 200px;
        width: auto;
      }
      .footer-content{
        height: 170px;
      }
      .num{
        font-size: 1.5rem;
        opacity: 0.4;
      }
      .num-par{
        font-size: 1.2rem;
      }
      .num-detail{
        font-size: 1.1rem;
        opacity: 0.6;
      }
      
    }
</style>

<footer class="footer">
    <div class="item-one header">
  <img src="../images/image-retro-pcs.jpg" alt="" />
    <div class="footer-content">
      <h1 class="num">01</h1>
      <p class="num-par">Reviving Retro PCs</p>
      <p class="num-detail">
        What happens when old PCs are given modern upgrades?
      </p>
    </div>
  </div>
  <div class="item-two">
  <img src="../images/image-top-laptops.jpg" alt="" />
    <div class="footer-content">
      <h1 class="num">02</h1>
      <p class="num-par">Top 10 Laptops of 2022</p>
      <p class="num-detail">
        Our best picks for various needs and budgets.
      </p>
</div>
  </div>
  <div class="item-three">
  <img src="../images/image-gaming-growth.jpg" alt="" />
    <div class="footer-content">
      <h1 class="num">03</h1>
      <p class="num-par">The Growth of Gaming</p>
      <p class="num-detail">
        How the pandemic has sparked fresh opportunities.
      </p>
    </div>
  </div>
</footer>
