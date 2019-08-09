[Autodesk Forge Viewer](https://forge.autodesk.com/api/viewer-cover-page/) type module for TypeScript ^3.5

**Sample application**: [autodesk-forge-viewer-sample](https://github.com/mazhuravlev/autodesk-forge-viewer-sample)

Usage
----

    import Autodesk from 'autodesk-forge-viewer';
    const autodesk: typeof Autodesk = (window as any).Autodesk;

 Use **Autodesk** as a type, and **autodesk** as a value

    // OK  
    const options: Autodesk.Viewing.InitializerOptions = { /* options here */ };
    
    // OK
    autodesk.Viewing.Initializer(options, () => {});
    
    // FAIL (Viewing is undefined)
    Autodesk.Viewing.Initializer(options, () => {});
