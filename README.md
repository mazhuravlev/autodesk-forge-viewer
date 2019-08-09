[Autodesk Forge Viewer](https://forge.autodesk.com/api/viewer-cover-page/) type module for TypeScript ^3.5

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
