# Frequently Asked Questions

## Installation Issues

### Q: npm install fails
**A:** Ensure you're using Node.js 16+, clear npm cache:
```bash
npm cache clean --force
npm install
```

### Q: Development server won't start
**A:** Check if port 8080 is in use:
```bash
lsof -i :8080
```

## Performance Issues

### Q: Low frame rate
**A:** Optimization suggestions:
- Reduce scene polygon count
- Optimize texture sizes
- Lower shadow quality
- Reduce number of physics objects

### Q: High memory usage
**A:** 
- Release unused resources promptly
- Use texture compression
- Limit simultaneously loaded models

## Development Issues

### Q: Model loading fails
**A:** Check:
- GLB file path is correct
- File is not corrupted
- Server MIME types are configured correctly

### Q: Physics collision incorrect
**A:** 
- Ensure collision mesh naming is correct
- Check physics material settings
- Verify collision body shapes

### Q: Character control abnormal
**A:** 
- Check input bindings
- Verify character state machine
- Confirm camera settings

## Browser Compatibility

### Supported Browsers
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### WebGL Requirements
- WebGL 2.0 support
- Sufficient GPU memory
- Hardware acceleration enabled

## Deployment Issues

### Q: Resource loading fails in production
**A:** 
- Configure correct CORS headers
- Ensure HTTPS environment
- Check resource paths

### Q: Poor performance on mobile devices
**A:** 
- Use low quality settings
- Reduce particle effects
- Optimize touch controls
