# PyCDocTemplate

## PyCDocTemplate Object

A document template class.  Encapsulates an MFC __CDocTemplate__ class

#### Methods


  - [DoCreateDoc](PyCDocTemplate.md#pycdoctemplatedocreatedoc)

    Creates an underlying document object.&nbsp;

  - [FindOpenDocument](PyCDocTemplate.md#pycdoctemplatefindopendocument)

    Returns an existing document with the specified file name.&nbsp;

  - [GetDocString](PyCDocTemplate.md#pycdoctemplategetdocstring)

    Retrieves a specific substring describing the document type.&nbsp;

  - [GetDocumentList](PyCDocTemplate.md#pycdoctemplategetdocumentlist)

    Return a list of all open documents.&nbsp;

  - [GetResourceID](PyCDocTemplate.md#pycdoctemplategetresourceid)

    Returns the resource ID in use.&nbsp;

  - [GetSharedMenu](PyCDocTemplate.md#pycdoctemplategetsharedmenu)

    Returns the shared menu object for all frames using this template.&nbsp;

  - [InitialUpdateFrame](PyCDocTemplate.md#pycdoctemplateinitialupdateframe)

    Calls the default OnInitialFrame handler.&nbsp;

  - [SetContainerInfo](PyCDocTemplate.md#pycdoctemplatesetcontainerinfo)

    Sets the resources to be used when an OLE 2 object is in-place activated.&nbsp;

  - [SetDocStrings](PyCDocTemplate.md#pycdoctemplatesetdocstrings)

    Assigns the document strings for the template.&nbsp;

  - [OpenDocumentFile](PyCDocTemplate.md#pycdoctemplateopendocumentfile)

    Opens a document file, creating a view and frame.&nbsp;

## [PyCDocTemplate.CreateNewDocument](#pycdoctemplate)Virtual

 __CreateNewDocument(__ )
Called to create a new document object.

## [PyCDocTemplate.CreateNewFrame](#pycdoctemplate)Virtual

 __CreateNewFrame(__ )
Called to create a new frame window.

## [PyCDocTemplate](#pycdoctemplate).DoCreateDoc

[PyCDocument](#pycdocument)= __DoCreateDoc( *fileName* __ )
Creates an underlying document object.

#### Parameters


  -  *fileName=None* : string

    The name of the file to load.

## [PyCDocTemplate](#pycdoctemplate).FindOpenDocument

[PyCDocument](#pycdocument)= __FindOpenDocument( *fileName* __ )
Returns an existing document with the specified file name.

#### Parameters


  -  *fileName* : string

    The fully qualified filename to search for.

## [PyCDocTemplate](#pycdoctemplate).GetDocString

string = __GetDocString( *docIndex* __ )
Retrieves a specific substring describing the document type.

#### Parameters


  -  *docIndex* : int

    The document index.  Must be one of the win32ui.CDocTemplate_* constants.

#### Comments
For more information on the doc strings, please see[PyCDocTemplate::SetDocStrings](PyCDocTemplate.md#pycdoctemplatesetdocstrings)

## [PyCDocTemplate](#pycdoctemplate).GetDocumentList

list = __GetDocumentList(__ )
Return a list of all open documents.

## [PyCDocTemplate](#pycdoctemplate).GetResourceID

 __GetResourceID(__ )
Returns the resource ID in use.

## [PyCDocTemplate](#pycdoctemplate).GetSharedMenu

[PyCMenu](#pycmenu)= __GetSharedMenu(__ )
Returns the shared menu object for all frames using this template.

#### MFC References


  - CWnd::m_hMenuShared

## [PyCDocTemplate](#pycdoctemplate).InitialUpdateFrame

 __InitialUpdateFrame( *frame*  *, doc*  *, bMakeVisible* __ )
Calls the default OnInitialFrame handler.

#### Parameters


  -  *frame=None* :[PyCFrameWnd](#pycframewnd)

    The frame window.

  -  *doc=None* :[PyCDocument](#pycdocument)

    A document for the frame.

  -  *bMakeVisible=1* : int

    Indicates of the frame should be shown.

#### See Also


  - [PyCDocTemplate.InitialUpdateFrame](PyCDocTemplate.md#pycdoctemplateinitialupdateframe_virtual)virtual method

## [PyCDocTemplate.InitialUpdateFrame](#pycdoctemplate)Virtual

 __InitialUpdateFrame( *frame*  *, frame*  *, bMakeVisible* __ )
Called to perform the initial frame update. 

The default behaviour is to call OnInitialUpdate on all views.

#### Parameters


  -  *frame* :[PyCFrameWnd](#pycframewnd)

    The frame window.

  -  *frame* :[PyCDocument](#pycdocument)

    The document attached to the frame.

  -  *bMakeVisible* : int

    Indicates if the frame should be made visible.

## [PyCDocTemplate.MatchDocType](#pycdoctemplate)Virtual

 __MatchDocType( *fileName*  *, fileType* __ )
Queries if the template can open the specified file name.

#### Parameters


  -  *fileName* : string

    The name of the file to open.

  -  *fileType* : int

    Only used on the mac.

#### Comments
This method should call PyCDocTemplate.FindOpenDocument to return an already open 

document if one exists, else it should return one of the win32ui.CDocTemplate_Confidence_* constants.

## [PyCDocTemplate](#pycdoctemplate).OpenDocumentFile

 __OpenDocumentFile( *filename*  *, bMakeVisible* __ )
Opens a document file, creating a view and frame.

#### Parameters


  -  *filename* : string

    Name of file to open, or None

  -  *bMakeVisible=1* : int

    Indicates if the document should be created visible.

## [PyCDocTemplate.OpenDocumentFile](#pycdoctemplate)Virtual

 __OpenDocumentFile(__ )
Called when a document file is to be opened.

## [PyCDocTemplate](#pycdoctemplate).SetContainerInfo

 __SetContainerInfo( *id* __ )
Sets the resources to be used when an OLE 2 object is in-place activated.

#### Parameters


  -  *id* : int

    The resource ID.

## [PyCDocTemplate](#pycdoctemplate).SetDocStrings

 __SetDocStrings( *docStrings* __ )
Assigns the document strings for the template.

#### Parameters


  -  *docStrings* : string

    The document strings.

#### Comments
The string must be a \\n seperated list of docstrings. 

The elements are: