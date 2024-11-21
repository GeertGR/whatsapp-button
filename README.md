# WhatsApp Button Component for Google Tag Manager

A floating WhatsApp button that can be easily implemented through Google Tag Manager (GTM). This component allows website visitors to start a WhatsApp conversation with one click.

## Google Tag Manager Implementation

1. **Create a Custom HTML Tag:**
   - Go to Google Tag Manager
   - Navigate to Tags > New > Custom HTML
   - Name your tag (e.g., "WhatsApp Button")

2. **Copy this code into the Custom HTML field:**
   ```html
   <style>
     #whatsapp-button {
       position: fixed;
       bottom: 20px;
       right: 20px;
       z-index: 9999;
       background-color: #25D366;
       border-radius: 50%;
       width: 60px;
       height: 60px;
       display: flex;
       justify-content: center;
       align-items: center;
       box-shadow: 0 2px 5px rgba(0, 0, 0, 0.25);
       transition: background-color 0.3s ease;
     }

     #whatsapp-button:hover {
       background-color: #128C7E;
     }

     #whatsapp-button img {
       width: 30px;
       height: 30px;
       filter: brightness(0) invert(1);
     }
   </style>

   <a href="https://wa.me/31612345678" target="_blank" id="whatsapp-button">
     <img src="https://cdn.jsdelivr.net/gh/twbs/icons/icons/whatsapp.svg" alt="WhatsApp" />
   </a>
   ```

3. **Configure Tag Settings:**
   - Set trigger to 'All Pages' or your preferred trigger
   - Support document.write: No
   - HTML validation: No

4. **Customize:**
   - Replace `31612345678` with your WhatsApp number (include country code, no '+' or spaces)
   - Adjust styling if needed

5. **Test and Publish:**
   - Test in GTM Preview mode
   - Verify on different devices and screen sizes
   - Publish when satisfied

## Customization Options

Modify these CSS properties as needed:
- Button position: `bottom` and `right` values
- Button size: `width` and `height`
- Colors: `background-color`
- Icon size: img `width` and `height`

## Browser Support
- Chrome
- Firefox
- Safari
- Edge
- Opera

## License
Free to use in both personal and commercial projects. No attribution required. 