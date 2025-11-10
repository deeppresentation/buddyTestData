# Test Data

This directory contains test data used by the test suite.

## Images

The `images/` directory contains local copies of all test images used in the test suite. These images are committed to git to ensure:

1. **Stable tests** - No dependency on external URLs that may change or become unavailable
2. **Offline testing** - Tests can run without internet connection
3. **No rate limiting** - Avoid 403/429 errors from external image services
4. **Consistent results** - Same images across all environments and developers

### Directory Structure

Images are organized by category matching the structure in `tests/_utils/test-data-loader.ts`:

```
images/
├── people/           # Portrait photos
├── personWithObject/ # People holding/using objects
├── animals/          # Animal photos
├── objects/          # Standalone objects
├── landscapes/       # Landscape photos
├── nature/           # Nature scenes
├── architecture/     # Buildings and structures
├── artistic/         # Abstract art and textures
└── format/           # Format-specific test images (jpg, png)
```

### Image Sources

Images are sourced from:
- **Wikimedia Commons** - Public domain images
- **Picsum Photos** - Free stock photos
- **Pravatar** - Avatar placeholders

All images are used under their respective licenses for testing purposes.