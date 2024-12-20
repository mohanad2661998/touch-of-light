<!DOCTYPE html>
<html lang="en">
    <title>Fastlane - PayPal Integration - Quick Start</title>

    <head>
        <link rel="stylesheet" href="styles.css" />
    </head>

    <body>
        <form>
            <h1>Fastlane - PayPal Integration - Quick Start</h1>

            <section id="customer" class="active visited">
                <div class="header">
                    <h2>Customer</h2>
                    <button
                        id="email-edit-button"
                        type="button"
                        class="edit-button"
                    >
                        Edit
                    </button>
                </div>
                <div class="summary"></div>
                <div class="email-container">
                    <fieldset class="email-input-with-watermark">
                        <input
                            id="email-input"
                            name="email"
                            type="email"
                            placeholder="Email"
                            autocomplete="email"
                        />
                        <div id="watermark-container"></div>
                    </fieldset>
                    <button
                        id="email-submit-button"
                        type="button"
                        class="submit-button"
                        disabled
                    >
                        Continue
                    </button>
                </div>
            </section>

            <hr />

            
            <section id="shipping">
                <div class="header">
                    <h2>Shipping</h2>
                    <button
                        id="shipping-edit-button"
                        type="button"
                        class="edit-button"
                    >
                        Edit
                    </button>
                </div>
                <div class="summary"></div>
                <fieldset>
                    <span>
                        <input
                            id="shipping-required-checkbox"
                            name="shipping-required"
                            type="checkbox"
                            checked
                        />
                        <label for="shipping-required-checkbox"
                            >This purchase requires shipping</label
                        >
                    </span>
                    <input
                        name="given-name"
                        placeholder="First name"
                        autocomplete="given-name"
                    />
                    <input
                        name="family-name"
                        placeholder="Last name"
                        autocomplete="family-name"
                    />
                    <input
                        name="address-line1"
                        placeholder="Street address"
                        autocomplete="address-line1"
                    />
                    <input
                        name="address-line2"
                        placeholder="Apt., ste., bldg. (optional)"
                        autocomplete="address-line2"
                    />
                    <input
                        name="address-level2"
                        placeholder="City"
                        autocomplete="address-level2"
                    />
                    <input
                        name="address-level1"
                        placeholder="State"
                        autocomplete="address-level1"
                    />
                    <input
                        name="postal-code"
                        placeholder="ZIP code"
                        autocomplete="postal-code"
                    />
                    <input
                        name="country"
                        placeholder="Country"
                        autocomplete="country"
                    />
                    <input
                        name="tel-country-code"
                        placeholder="Country calling code"
                        autocomplete="tel-country-code"
                    />
                    <input
                        name="tel-national"
                        type="tel"
                        placeholder="Phone number"
                        autocomplete="tel-national"
                    />
                </fieldset>
                <button
                    id="shipping-submit-button"
                    type="button"
                    class="submit-button"
                >
                    Continue
                </button>
            </section>
            
            <hr />

            <section id="payment">
                <div class="header">
                    <h2>Payment</h2>
                    <button
                        id="payment-edit-button"
                        type="button"
                        class="edit-button"
                    >
                        Edit
                    </button>
                </div>
                <fieldset>
                    <div id="payment-component"></div>
                </fieldset>
            </section>

            <button id="checkout-button" type="button" class="submit-button">
                Checkout
            </button>
        </form>

        
        <script
            src="https://www.paypal.com/sdk/js?client-id=AZdvTdjKqgkC2ba6Z6VFE_xovlKUaSbUmZhnd0CYMmEnxANHHJVrFVzQTZ7UERtxXlqSg2KU0_IFgV7V&components=buttons%2Cfastlane"
            data-sdk-client-token="eyJraWQiOiJkMTA2ZTUwNjkzOWYxMWVlYjlkMTAyNDJhYzEyMDAwMiIsInR5cCI6IkpXVCIsImFsZyI6IkVTMjU2In0.eyJpc3MiOiJodHRwczovL2FwaS5zYW5kYm94LnBheXBhbC5jb20iLCJhdWQiOlsiaHR0cHM6Ly9hcGkuYnJhaW50cmVlZ2F0ZXdheS5jb20iLCJwYXlwYWwuY29tIl0sInN1YiI6Ikw1TUg4NEhRTExGNUciLCJhY3IiOlsiY2xpZW50Il0sInNjb3BlIjpbXSwib3B0aW9ucyI6e30sImF6IjoiY2NnMTguc2xjIiwiZXh0ZXJuYWxfaWQiOlsiUGF5UGFsOkw1TUg4NEhRTExGNUciLCJCcmFpbnRyZWU6YjNubjd3czg1azZ5Ynl6aCJdLCJleHAiOjE3MzIyMjY1NzIsImlhdCI6MTczMjIyNTY3MiwianRpIjoiVTJBQUpmdDJFa3BQWUI0cXJKTWwtcTNiWDNrM2hsX3B1TWg5ZTVpbUREWWM4OVZuNmRXYWgwQlVkSElCUWVXc081UDhtNW5Lc0VNRlNZclJOaUJwcHZfRHlpc1hOaERxZklqMHJXdGlsSmZpcHlkazQ2M0xRV0tER3pqdy1tLVEifQ.IPAjfOSlnsqH1-CWEaGbW1EGWgd7pW_mWMiFRGFY12dj1vsEZ34IGH2LI5zvB_eOtnPD-6QZCRmb1aCMnoOt7A"
            data-sdk-integration-source="developer-studio"
            defer
        ></script>
        
        <script src="app.js" defer></script>
    </body>
</html>
