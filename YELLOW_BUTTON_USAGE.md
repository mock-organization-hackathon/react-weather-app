# Yellow Button Usage Guide

## Overview
A new yellow button variant has been added to the weather application. This button provides an alternative styling option while maintaining the same functionality as existing buttons.

## Usage

### Basic Usage
```jsx
import Button from './components/button';

function MyComponent() {
  return (
    <Button
      text="Weather Alert"
      className="brand-btn-yellow width-toggle"
      onClick={() => console.log('Yellow button clicked!')}
    />
  );
}
```

### Available CSS Classes
- `brand-btn-yellow` - The main yellow button styling
- Combine with existing utility classes like `width-toggle`, `width-toggle-2`, etc.

## Styling Details
- **Background Color**: #ffc107 (Bootstrap-inspired yellow)
- **Text Color**: Black (#000) for proper contrast
- **Hover Effect**: Darker yellow (#e0a800)
- **Border Radius**: 30px (consistent with other brand buttons)
- **Padding**: 15px
- **Transition**: 0.9s smooth transition

## Examples

### Standard Yellow Button
```jsx
<Button
  text="Get Weather Updates"
  className="brand-btn-yellow width-toggle"
  onClick={handleWeatherUpdate}
/>
```

### Yellow Button with Custom Styling
```jsx
<Button
  text="Emergency Alert"
  className="brand-btn-yellow width-toggle-2"
  style={{ fontSize: '16px', fontWeight: 'bold' }}
  onClick={handleEmergencyAlert}
/>
```

## Accessibility
- High contrast ratio between yellow background and black text
- Keyboard accessible (inherits from base Button component)
- Screen reader friendly with proper text content

## Browser Support
- Modern browsers supporting CSS custom properties
- Fallback colors available if CSS variables not supported
