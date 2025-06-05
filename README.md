# JSON Form Builder

A powerful, user-friendly web application for creating professional forms without coding. Built specifically for organisations that need to digitise forms and streamline data collection workflows.

## 🚀 Features

### No-Code Form Creation
- **Drag & Drop Interface** - Reorder questions with simple drag and drop
- **Live Preview** - See your form as you build it
- **Professional Styling** - Clean, modern interface suitable for business use
- **JSON Export** - Generate clean, ready-to-implement JSON code

### Comprehensive Field Types
- **Text Fields** - Single line and multi-line text inputs
- **Selection Fields** - Dropdowns, radio buttons, and checkboxes
- **Date/Time Pickers** - Professional date and time selection
- **Digital Signatures** - Built-in signature capture support
- **Yes/No Checkboxes** - Boolean field support
- **Section Headers** - Organise forms with fieldsets and grouping

### Smart Form Logic
- **Required/Optional Fields** - Flexible validation control
- **Professional Validation** - Built-in form validation rules
- **Help Text Support** - Add guidance for form users
- **Option Management** - Easy configuration for dropdown and radio fields

### Export & Integration
- **Clean JSON Output** - Standards-compliant JSON Schema format
- **Copy to Clipboard** - One-click copying for easy integration
- **Reset Functionality** - Clear and start over with confirmation
- **Professional Branding** - Customisable styling and branding

## 🎯 Demo

**Live Demo:** [https://bzymind.github.io/JSON_Form_Builder/](https://bzymind.github.io/JSON_Form_Builder/)

## 📋 Use Cases

- **Assessment Forms** - Digital care assessments, evaluations, surveys
- **Data Collection** - Professional questionnaires and intake forms
- **Business Forms** - Application forms, feedback forms, registration
- **Research** - Survey forms, data gathering instruments
- **Compliance** - Audit forms, inspection checklists, documentation

## 🛠️ Technology Stack

- **Frontend** - HTML5, CSS3, JavaScript (ES6+)
- **UI Framework** - Bootstrap 3.4.1
- **Form Library** - JSONForm 2.2.5
- **Dependencies** - jQuery, Underscore.js, Sortable.js
- **Hosting** - GitHub Pages (Static hosting)

## 🚀 Quick Start

### Option 1: Use Online (Recommended)
1. Visit the [live demo](https://bzymind.github.io/JSON_Form_Builder/)
2. Start building your form immediately
3. Copy the generated JSON code
4. Integrate into your application

### Option 2: Download and Run Locally
1. **Clone the repository**
   ```bash
   git clone https://github.com/bzymind/JSON_Form_Builder.git
   cd JSON_Form_Builder
   ```

2. **Open in browser**
   ```bash
   # Simply open index.html in your web browser
   open index.html  # macOS
   start index.html # Windows
   ```

3. **Or serve locally**
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Then visit http://localhost:8000
   ```

## 📖 Usage Guide

### Building Your First Form

1. **Set Form Title** - Give your form a clear, descriptive name
2. **Add Questions** - Use the "Add New Question" panel to create fields:
   - Enter question text
   - Select appropriate field type
   - Mark as required/optional
   - Add help text if needed
3. **Configure Options** - For dropdowns/radio buttons, add your options
4. **Organise Structure** - Use section headers to group related questions
5. **Preview Live** - Check the "Live Preview" panel to see your form
6. **Generate JSON** - Click "Generate JSON Form Code" when ready
7. **Copy & Integrate** - Use the copy button to get your JSON code

### Field Type Guide

| Field Type | Best Used For | Options Required |
|------------|---------------|------------------|
| **Single Line Text** | Names, short answers | No |
| **Multi-line Text** | Comments, descriptions | No |
| **Dropdown List** | >5 options, long lists | Yes |
| **Radio Buttons** | ≤5 options, single choice | Yes |
| **Checkboxes** | Multiple selections | Yes |
| **Date Picker** | Date selection | No |
| **Time Picker** | Time selection | No |
| **Yes/No Checkbox** | Boolean questions | No |
| **Digital Signature** | Signature capture | No |
| **Section Header** | Form organisation | No |

### Advanced Features

- **Drag & Drop** - Reorder questions by dragging
- **Clear & Reset** - Start over with confirmation dialog
- **Form Validation** - Built-in required field validation
- **Professional Styling** - Consistent, business-ready appearance

## 🔧 Integration

The generated JSON follows the JSONForm library specification and can be integrated into any application that supports JSON Schema forms.

### Example Integration
```javascript
// Use the generated JSON in your application
$('#form-container').jsonForm({
  schema: generatedSchema,
  form: generatedForm,
  onSubmit: function(errors, values) {
    if (errors) {
      console.log('Validation errors:', errors);
    } else {
      console.log('Form data:', values);
      // Process form submission
    }
  }
});
```

## 🎨 Customisation

The application uses CSS custom properties for easy theming:

```css
:root {
  --primary-color: #62bb46;
  --secondary-color: #1E1869;
  --background-color: #ffffff;
  --text-color: #4d4d4d;
}
```

## 📱 Browser Support

- **Chrome** 60+
- **Firefox** 60+
- **Safari** 12+
- **Edge** 79+
- **Mobile** iOS Safari 12+, Android Chrome 60+

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Guidelines
- Maintain existing code style
- Test across multiple browsers
- Update documentation as needed
- Keep commits focused and descriptive

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙋‍♂️ Support

- **Issues** - Report bugs or request features via [GitHub Issues](https://github.com/bzymind/JSON_Form_Builder/issues)
- **Discussions** - Ask questions in [GitHub Discussions](https://github.com/bzymind/JSON_Form_Builder/discussions)

## 🎉 Acknowledgments

- [JSONForm](https://github.com/jsonform/jsonform) - Core form rendering library
- [Bootstrap](https://getbootstrap.com/) - UI framework
- [jQuery](https://jquery.com/) - JavaScript library
- [SortableJS](https://sortablejs.github.io/Sortable/) - Drag and drop functionality

## 📊 Project Stats

![GitHub stars](https://img.shields.io/github/stars/bzymind/JSON_Form_Builder?style=social)
![GitHub forks](https://img.shields.io/github/forks/bzymind/JSON_Form_Builder?style=social)
![GitHub issues](https://img.shields.io/github/issues/bzymind/JSON_Form_Builder)
![GitHub license](https://img.shields.io/github/license/bzymind/JSON_Form_Builder)

---

**Made with ❤️ for organisations digitising their workflows**
