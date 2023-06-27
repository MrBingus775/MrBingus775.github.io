---
layout: page
title: Contact
hide_title: true
permalink: /contact/
path: /contact/
order: 4
---

<div class="container mt-5">
    <div class="row justify-content-center">
        <div class="col-lg-6">
            <h2 class="mb-4">Contact Pantheon Insights</h2>

            <p>
              Please use the form below to inquire about Pantheon Insights speaking at your event, request consulting services, or address general queries: 
            </p>

            <br/>

            <form id="contactForm">
                <div class="mb-3">
                    <label for="fullName" class="form-label">Full Name</label>
                    <input type="text" class="form-control" id="fullName" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" id="email" required>
                </div>
                <div class="mb-3">
                    <label for="phone" class="form-label">Phone number</label>
                    <input type="tel" class="form-control" id="phone" required>
                </div>
                <div class="mb-3">
                    <label for="message" class="form-label">Your message</label>
                    <textarea class="form-control" id="message" rows="5" required></textarea>
                </div>
                <button type="submit" class="btn btn-primary">Submit</button>
            </form>
        </div>
    </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/web3forms/dist/web3forms.js"></script>
<script>
    document.addEventListener('DOMContentLoaded', function () {
        const contactForm = document.getElementById('contactForm');

        contactForm.addEventListener('submit', function (e) {
            e.preventDefault();

            const fullName = document.getElementById('fullName').value;
            const email = document.getElementById('email').value;
            const phone = document.getElementById('phone').value;
            const message = document.getElementById('message').value;

            const formData = {
                fullName,
                email,
                phone,
                message
            };

            // Submit the form using Web3Forms
            Web3Forms.submitForm({
                formId: 'your-form-id',
                apiKey: 'your-api-key',
                data: formData,
                onSuccess: function () {
                    alert('Thank you for your message! We will get back to you soon.');
                    contactForm.reset();
                },
                onError: function () {
                    alert('An error occurred while submitting the form. Please try again later.');
                }
            });
        });
    });
</script>
