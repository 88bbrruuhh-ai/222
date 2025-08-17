# Simple PagesCMS Website

A basic website template with PagesCMS integration for easy content management.

## 📁 Project Structure

```
├── .pages.yml          # PagesCMS configuration
├── index.html          # Main webpage
├── content/            # Editable content
│   ├── pages/          # Static pages
│   └── posts/          # Blog posts
├── data/              # Site configuration data
│   └── site.json      # Global site settings
└── media/             # Media assets
    ├── blog/          # Blog images
    └── images/        # General images
```

## 🚀 Getting Started

### 1. Open the Website

Simply open `index.html` in your web browser to view the basic website.

### 2. Set Up PagesCMS

To enable content editing through PagesCMS:

1. **Install PagesCMS**: Follow the [official setup guide](https://pagescms.org)
2. **Connect Repository**: Link your GitHub repository to PagesCMS
3. **Deploy**: Host PagesCMS on your preferred platform (Vercel, Netlify, etc.)

### 3. Content Management

Once PagesCMS is set up, you can:

- **Edit Pages**: Modify content in `content/pages/`
- **Manage Blog Posts**: Add/edit posts in `content/posts/`
- **Update Site Settings**: Modify global settings in `data/site.json`
- **Upload Media**: Manage images and files through the interface

## 📝 Content Types

### Pages
- Static pages like Home, About, Contact
- Fields: title, description, cover image, content

### Blog Posts
- Dynamic blog content
- Fields: title, author, tags, excerpt, cover image, content
- Automatic date and publishing controls

### Site Settings
- Global website configuration
- Logo, social media links, site description
- URL and metadata settings

## 🎨 Customization

### Adding New Fields

Edit `.pages.yml` to add new fields:

```yaml
fields:
  - name: new_field
    label: New Field
    type: string
    required: false
```

### Field Types Available

- `string`: Single line text
- `text`: Multi-line text
- `rich-text`: WYSIWYG editor
- `image`: Image upload/selection
- `file`: File upload/selection
- `date`: Date picker
- `boolean`: Toggle switch
- `select`: Dropdown with options
- `number`: Numeric input
- `object`: Grouped fields

### Media Configuration

The current setup supports:

- Images in `/media/images/`
- Blog images in `/media/blog/`
- All media accessible at `/media/` URL path

## 🔧 Integration with Static Site Generators

This setup works with popular static site generators:

- **11ty**: Use the frontmatter and content structure
- **Jekyll**: Compatible with Jekyll's post format
- **Hugo**: Adapt the frontmatter format as needed
- **Gatsby**: Use with markdown transformer plugins
- **Next.js**: Integrate with `getStaticProps`

## 📚 PagesCMS Features Used

This template demonstrates:

- ✅ **Content Collections**: Blog posts and pages
- ✅ **Rich Text Editing**: WYSIWYG content editor
- ✅ **Media Management**: Image and file uploads
- ✅ **Custom Fields**: Various field types
- ✅ **Settings Management**: Global site configuration
- ✅ **Validation**: Required fields and patterns
- ✅ **Multiple Selection**: Tags and categories
- ✅ **Date Handling**: Publication dates

## 🌟 Next Steps

1. **Customize Design**: Modify `index.html` styling
2. **Add More Content Types**: Extend `.pages.yml` configuration
3. **Integrate Build Process**: Connect with your static site generator
4. **Deploy**: Host your website and PagesCMS
5. **Train Team**: Show content creators how to use the interface

## 📖 Documentation

- [PagesCMS Official Docs](https://pagescms.org)
- [Configuration Reference](https://pagescms.org/docs/configuration)
- [Field Types](https://pagescms.org/docs/configuration)

---

**Happy content managing! 🎉**
