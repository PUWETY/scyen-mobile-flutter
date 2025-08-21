# Scyen Flutter App (slim)
Add this step in workflow before build (if android/ not present):
```yaml
- name: Ensure Flutter project structure
  run: |
    if [ ! -d "android" ]; then
      flutter create .
    fi
```
