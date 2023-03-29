<script>
  import iconReaction from '$lib/assets/images/icon-reaction.svg'
  import iconMemory from '$lib/assets/images/icon-memory.svg'
  import iconVerbal from '$lib/assets/images/icon-verbal.svg'
  import iconVisual from '$lib/assets/images/icon-visual.svg'
</script>

<main>
  <div class="result">
    <div class="heading">
      Your Result
    </div>
    <div class="score">
      <div class="your-score">
        76
      </div>
      <div class="out-of-possible">
        of 100
      </div>
    </div>
    <div class="message">
      Great
    </div>
    <p class="narrative">
      Your performance exceed 65% of the people conducting the test here!
    </p>
  </div>
  <div class="summary">
    <div class="heading">Summary</div>
    <ul>
      <li>
        <div>
          <div class="icon">
            <img
            src={iconReaction}
            alt=""
          ></div>
          <div class="label">Reaction</div>
          <div class="score">
            <span>80</span>
            <span>/</span>
            <span>100</span>
          </div>
        </div>
      </li>
      <li>
        <div>
          <div class="icon">
            <img
            src={iconMemory}
            alt=""
          ></div>
          <div class="label">Memory</div>
          <div class="score">
            <span>92</span>
            <span>/</span>
            <span>100</span>
          </div>
        </div>
      </li>
      <li>
        <div>
          <div class="icon">
            <img
              src={iconVerbal}
              alt=""
            ></div>
          <div class="label">Verbal</div>
          <div class="score">
            <span>61</span>
            <span>/</span>
            <span>100</span>
          </div>
        </div>
      </li>
      <li>
        <div>
          <div class="icon">
            <img
              src={iconVisual}
              alt=""
            ></div>
          <div class="label">Visual</div>
          <div class="score">
            <span>73</span>
            <span>/</span>
            <span>100</span>
          </div>
        </div>
      </li>
    </ul>
    <button>Continue</button>
  </div>
</main>

<style lang="scss">
  .result {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 356px;
    background: linear-gradient(180deg, #7755FF 0%, #6943FF 0.01%, #2F2CE9 100%);
    color: var(--c-white);
    box-shadow: 0 30px 60px rgba(61, 108, 236, 0.15);
    border-radius: 0 0 32px 32px;

    > * {
      text-align: center;
    }

    .heading {
      font-weight: var(--fw-bold);
      line-height: 1.4375rem;
      color: var(--c-light-lavender);
      padding-top: 1.5rem;
    }

    .score {
      margin-top: 1.5rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      width: 8.75rem;
      height: 8.75rem;
      border-radius: 50%;
      background: linear-gradient(180deg, #4D21C9 0%, rgba(37, 33, 201, 0) 100%, rgba(37, 33, 201, 0) 100%);

      .your-score {
        font-weight: var(--fw-extra-bold);
        margin-top: 0.3rem;
        font-size: 3.5rem;
        line-height: 4.5rem;
      }

      .out-of-possible {
        opacity: 0.52;
        font-weight: var(--fw-bold);
        color: var(--c-light-lavender);
        font-size: 1rem;
        line-height: 1.3125rem;
      }
    }

    .message {
      padding-top: 1.5rem;
      font-weight: 700;
      font-size: 24px;
      line-height: 31px;
    }

    .narrative {
      padding-top: .5rem;
      font-weight: var(--fw-medium);
      font-size: 1rem;
      color: var(--c-light-lavender);
      padding-left: 57px;
      padding-right: 57px;
      line-height: 21px;
    }

    .summary {
      ul {
        list-style: none;
        padding: 0;
        display: flex;
        gap: 1rem;

        li {
          div {
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: space-between;
          }
        }
      }
    }
  }
</style>
