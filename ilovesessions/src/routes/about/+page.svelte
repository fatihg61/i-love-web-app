<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import { onMount } from 'svelte';
        
        let showPopup = false;
        
        onMount(() => {
          const donateButton = document.querySelector('#donate-button');
        
          donateButton.addEventListener('click', () => {
            showPopup = true;
          });
        });
        
        function closePopup() {
          showPopup = false;
        }
</script>

<Header />

<main>
                <button id="donate-button">Donate</button>
        
        {#if showPopup}
          <div class="popup">
            <h2>Sponsor Donation</h2>
            <p>Please enter your credit card information to make a donation.</p>
        
            <form>
              <label for="name">Name:</label>
              <input type="text" id="name" required>
        
              <label for="creditCardNumber">Credit Card Number:</label>
              <input type="number" id="creditCardNumber" required>
        
              <label for="expirationDate">Expiration Date:</label>
              <input type="date" id="expirationDate" required>
        
              <label for="cvv">CVV:</label>
              <input type="number" id="cvv" required>
        
              <button type="submit">Donate</button>
            </form>
        
            <button onclick="openPopup()">Click me</button>
          </div>
        {/if}
</main>

<Footer />

<style>
        .popup {
          position: fixed;
          top: 50%;
          left: 50%;
          transform: translate(-50%, -50%);
          width: 400px;
          background-color: #fff;
          padding: 20px;
          border: 1px solid #ccc;
          box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }
        
        .popup h2 {
          text-align: center;
          margin-bottom: 20px;
        }
        
        .popup form {
          display: flex;
          flex-direction: column;
          margin-bottom: 20px;
        }
        
        .popup label {
          display: block;
          margin-bottom: 5px;
        }
        
        .popup input {
          width: 100%;
          padding: 5px;
          border: 1px solid #ccc;
        }
        
        .popup button {
          padding: 5px 10px;
          border: 1px solid #ccc;
          cursor: pointer;
        }
</style>