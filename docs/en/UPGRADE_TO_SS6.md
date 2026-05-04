# Upgrade to Silverstripe CMS 6

## Dependency Changes

### ⚠️ BREAKING CHANGE: Framework Version

- **Replace** `silverstripe/recipe-core: ^4.0 || ^5.0` with `silverstripe/recipe-core: ^6.0`
- This package now requires Silverstripe CMS 6.x

### **🚨 CRITICAL REVIEW REQUIRED: Missing Compatibility Package**

**The `sunnysideup/silverstripe-4-5-compatibility` dependency has been removed from `require` but is marked as "yet-to-update" with reason "no-compatible-stable-release".**

**You must:**
1. Verify if your project still depends on this compatibility package
2. Check if there is now a stable SS6-compatible version available
3. If no compatible version exists, audit your codebase for any features relying on this package and refactor them
4. Remove the `yet-to-update` section once resolved

This is not standard composer.json syntax and will need manual resolution before your project is production-ready.
