# PyCRichEditCtrl

## PyCRichEditCtrl Object

A windows Rich Text edit control.  Encapsulates an MFC __CRichEditCtrl__ class.  Derived from a[PyCControl](#pyccontrol)object.

#### Methods


  - [Clear](PyCRichEditCtrl.md#pycricheditctrlclear)

    Clears all text from an edit control.&nbsp;

  - [Copy](PyCRichEditCtrl.md#pycricheditctrlcopy)

    Copy the selection to the clipboard.&nbsp;

  - [CreateWindow](PyCRichEditCtrl.md#pycricheditctrlcreatewindow)

    Creates a rich edit control.&nbsp;

  - [Cut](PyCRichEditCtrl.md#pycricheditctrlcut)

    Cut the selection, and place it in the clipboard.&nbsp;

  - [FindText](PyCRichEditCtrl.md#pycricheditctrlfindtext)

    Finds text in the control&nbsp;

  - [GetCharPos](PyCRichEditCtrl.md#pycricheditctrlgetcharpos)

    Returns te location of the top-left corner of the specified character.&nbsp;

  - [GetDefaultCharFormat](PyCRichEditCtrl.md#pycricheditctrlgetdefaultcharformat)

    Returns the current default character formatting attributes in this __PyCRichEditCtrl__ object.&nbsp;

  - [GetEventMask](PyCRichEditCtrl.md#pycricheditctrlgeteventmask)

    Returns the current event mask.&nbsp;

  - [GetSelectionCharFormat](PyCRichEditCtrl.md#pycricheditctrlgetselectioncharformat)

    Returns the character formatting attributes of the current selection in this __PyCRichEditCtrl__ object.&nbsp;

  - [GetFirstVisibleLine](PyCRichEditCtrl.md#pycricheditctrlgetfirstvisibleline)

    Returns zero-based index of the topmost visible line.&nbsp;

  - [GetParaFormat](PyCRichEditCtrl.md#pycricheditctrlgetparaformat)

    Returns the formatting of the current paragraph.&nbsp;

  - [GetSel](PyCRichEditCtrl.md#pycricheditctrlgetsel)

    Returns the selection.&nbsp;

  - [GetSelText](PyCRichEditCtrl.md#pycricheditctrlgetseltext)

    Returns the currently selected text&nbsp;

  - [GetTextLength](PyCRichEditCtrl.md#pycricheditctrlgettextlength)

    Returns the length of the text in the control.&nbsp;

  - [GetLine](PyCRichEditCtrl.md#pycricheditctrlgetline)

    Returns a specified line.&nbsp;

  - [GetModify](PyCRichEditCtrl.md#pycricheditctrlgetmodify)

    Determines if the control has been modified.&nbsp;

  - [GetLineCount](PyCRichEditCtrl.md#pycricheditctrlgetlinecount)

    Returns the number of lines in an edit control.&nbsp;

  - [LimitText](PyCRichEditCtrl.md#pycricheditctrllimittext)

    Sets max length of text that user can enter&nbsp;

  - [LineFromChar](PyCRichEditCtrl.md#pycricheditctrllinefromchar)

    Returns the line number of a given character.&nbsp;

  - [LineIndex](PyCRichEditCtrl.md#pycricheditctrllineindex)

    Returns the line index&nbsp;

  - [LineScroll](PyCRichEditCtrl.md#pycricheditctrllinescroll)

    Scroll the control vertically and horizontally&nbsp;

  - [Paste](PyCRichEditCtrl.md#pycricheditctrlpaste)

    Pastes the contents of the clipboard into the edit control.&nbsp;

  - [ReplaceSel](PyCRichEditCtrl.md#pycricheditctrlreplacesel)

    Replace the selection with the specified text.&nbsp;

  - [SetBackgroundColor](PyCRichEditCtrl.md#pycricheditctrlsetbackgroundcolor)

    Sets the background color for the control.&nbsp;

  - [SetDefaultCharFormat](PyCRichEditCtrl.md#pycricheditctrlsetdefaultcharformat)

    Sets the current default character formatting attributes in this PyCRichEditCtrl object.&nbsp;

  - [SetEventMask](PyCRichEditCtrl.md#pycricheditctrlseteventmask)

    Sets the event motification mask.&nbsp;

  - [SetSelectionCharFormat](PyCRichEditCtrl.md#pycricheditctrlsetselectioncharformat)

    Sets the character formatting attributes for the selection in this PyCRichEditCtrl object.&nbsp;

  - [SetModify](PyCRichEditCtrl.md#pycricheditctrlsetmodify)

    Sets the modified flag.&nbsp;

  - [SetOptions](PyCRichEditCtrl.md#pycricheditctrlsetoptions)

    Sets options for the control.&nbsp;

  - [SetParaFormat](PyCRichEditCtrl.md#pycricheditctrlsetparaformat)

    Sets the paragraph formatting.&nbsp;

  - [SetReadOnly](PyCRichEditCtrl.md#pycricheditctrlsetreadonly)

    Set the read only status of an edit control.&nbsp;

  - [SetSel](PyCRichEditCtrl.md#pycricheditctrlsetsel)

    Changes the selection in an edit control.&nbsp;

  - [SetSelAndCharFormat](PyCRichEditCtrl.md#pycricheditctrlsetselandcharformat)

    Sets the selection and the char format.&nbsp;

  - [SetTargetDevice](PyCRichEditCtrl.md#pycricheditctrlsettargetdevice)

    Sets the target device for the control&nbsp;

  - [StreamIn](PyCRichEditCtrl.md#pycricheditctrlstreamin)

    Invokes a callback to stream data into the control.&nbsp;

  - [StreamOut](PyCRichEditCtrl.md#pycricheditctrlstreamout)

    Invokes a callback to stream data out of the control.&nbsp;

## [PyCRichEditCtrl](#pycricheditctrl).Clear

int = __Clear(__ )
Clears all text in an edit control.

#### MFC References


  - CRichEditCtrl::Clear

## [PyCRichEditCtrl](#pycricheditctrl).Copy

 __Copy(__ )
Copys the current selection to the clipboard.

#### MFC References


  - CRichEditCtrl::Copy

## [PyCRichEditCtrl](#pycricheditctrl).CreateWindow

 __CreateWindow( *style*  *, rect*  *, parent*  *, id* __ )
Creates a rich edit control window.

#### Parameters


  -  *style* : int

    The control style

  -  *rect* : int,int,int,int

    The position of the control

  -  *parent* :[PyCWnd](#pycwnd)

    The parent window.  Must not be None

  -  *id* : int

    The control ID

## [PyCRichEditCtrl](#pycricheditctrl).Cut

 __Cut(__ )
Cuts the current selection to the clipboard.

#### MFC References


  - CRichEditCtrl::Cut

## [PyCRichEditCtrl](#pycricheditctrl).FindText

int, (start, end) = __FindText( *charPos* __ )
Finds text in the control

#### Parameters


  -  *charPos* : int

    The character position

## [PyCRichEditCtrl](#pycricheditctrl).GetCharPos

(tuple) = __GetCharPos( *charPos* __ )
Returns the location of the top-left corner of the character specified by charPos.

#### Parameters


  -  *charPos* : int

    The character position

#### Return Value
The return value is a __win32ui::CHARFORMAT tuple__ 

## [PyCRichEditCtrl](#pycricheditctrl).GetDefaultCharFormat

(tuple) = __GetDefaultCharFormat(__ )
Returns the current default character formatting attributes in this[PyCRichEditCtrl](#pycricheditctrl)object.

#### MFC References


  - CRichEditCtrl::GetDefaultCharFormat

#### Return Value
The return value is a __win32ui::CHARFORMAT tuple__ 

## [PyCRichEditCtrl](#pycricheditctrl).GetEventMask

int = __GetEventMask(__ )
Returns the current event mask.

#### MFC References


  - CRichEditCtrl::GetEventMask

## [PyCRichEditCtrl](#pycricheditctrl).GetFirstVisibleLine

int = __GetFirstVisibleLine(__ )
Returns zero-based index of the topmost visible line.

#### MFC References


  - CRichEditCtrl::GetFirstVisibleLine

#### Return Value
The zero-based index of the topmost visible line. For single-line edit controls, the return value is 0.

## [PyCRichEditCtrl](#pycricheditctrl).GetLine

int = __GetLine( *lineNo* __ )
Returns the text in a specified line.

#### Parameters


  -  *lineNo=current* : int

    Contains the zero-based index value for the desired line.

#### Comments
This function is not an MFC wrapper.

## [PyCRichEditCtrl](#pycricheditctrl).GetLineCount

int = __GetLineCount(__ )
Gets the number of lines in an edit control.

#### MFC References


  - CRichEditCtrl::GetLineCount

#### Return Value
The number of lines in the buffer.  If the control is empty, the return value is 1.

## [PyCRichEditCtrl](#pycricheditctrl).GetModify

int = __GetModify(__ )
Nonzero if the text in this control has been modified; otherwise 0.

#### MFC References


  - CRichEditCtrl::GetModify

## [PyCRichEditCtrl](#pycricheditctrl).GetParaFormat

(tuple) = __GetParaFormat(__ )
Returns the current paragraph formatting attributes.

#### MFC References


  - CRichEditCtrl::GetParaFormat

#### Return Value
The return value is a __win32ui::PARAFORMAT tuple__ 

## [PyCRichEditCtrl](#pycricheditctrl).GetSel

(start, end) = __GetSel(__ )
Returns the start and end of the current selection.

#### MFC References


  - CRichEditCtrl::GetSel

#### Return Value
The return tuple is (the first character in the current selection, first nonselected character past the end of the current selection)

## [PyCRichEditCtrl](#pycricheditctrl).GetSelText

string = __GetSelText(__ )
Returns the currently selected text

## [PyCRichEditCtrl](#pycricheditctrl).GetSelectionCharFormat

(tuple) = __GetSelectionCharFormat(__ )
Returns the character formatting of the selection.

#### MFC References


  - CRichEditCtrl::GetSelectionCharFormat

## [PyCRichEditCtrl](#pycricheditctrl).GetTextLength

int = __GetTextLength(__ )
Returns the length of the text in the control.

#### MFC References


  - CRichEditCtrl::GetTextLength

## [PyCRichEditCtrl](#pycricheditctrl).LimitText

 __LimitText( *nChars* __ )
Sets max length of text that user can enter

#### Parameters


  -  *nChars=0* : int

    Specifies the length (in bytes) of the text that the user can enter. If this parameter is 0, the text length is set to 

UINT_MAX bytes. This is the default behavior.

#### MFC References


  - CRichEditCtrl::LimitText

## [PyCRichEditCtrl](#pycricheditctrl).LineFromChar

int = __LineFromChar( *charNo* __ )
Returns the line number of the specified character.

#### Parameters


  -  *charNo=-1* : int

    Contains the zero-based index value for the desired character in the text of the edit 

control, or -1.  If -1, then it specifies the current line.

#### MFC References


  - CRichEditCtrl::LineFromChar

#### Return Value
The zero-based line number of the line containing the character index specified by charNo. 

If charNo is -1, the number of the line that contains the first character of the selection is returned. 

If there is no selection, the current line number is returned.

## [PyCRichEditCtrl](#pycricheditctrl).LineIndex

int = __LineIndex( *lineNo* __ )
Retrieves the character index of a line within a multiple-line edit control.

#### Parameters


  -  *lineNo=-1* : int

    Contains the index value for the desired line in the text 

of the edit control, or contains -1.  If -1, then it specifies the current line.

#### Comments
This method only works on multi-linr edit controls.

#### MFC References


  - CRichEditCtrl::LineIndex

#### Return Value
The character index of the line specified in lineNo, or -1 if 

the specified line number is greater then the number of lines in 

the edit control.

## [PyCRichEditCtrl](#pycricheditctrl).LineScroll

int = __LineScroll( *nLines*  *, nChars* __ )
Scroll the control vertically and horizontally

#### Parameters


  -  *nLines* : int

    Specifies the number of lines to scroll vertically.

  -  *nChars=0* : int

    Specifies the number of character positions to scroll horizontally. This value is ignored if the edit control has either the 

ES_RIGHT or ES_CENTER style.

#### Comments
This method only works on multi-linr edit controls.

#### MFC References


  - CRichEditCtrl::LineScroll

## [PyCRichEditCtrl](#pycricheditctrl).Paste

 __Paste(__ )
Pastes the contents of the clipboard into the control.

#### MFC References


  - CRichEditCtrl::Paste

## [PyCRichEditCtrl](#pycricheditctrl).ReplaceSel

 __ReplaceSel( *text* __ )
Replaces the selection with the specified text.

#### Parameters


  -  *text* : string

    The text to replace the selection with.

#### MFC References


  - CRichEditCtrl::ReplaceSel

## [PyCRichEditCtrl](#pycricheditctrl).SetBackgroundColor

int = __SetBackgroundColor( *bSysColor*  *, cr* __ )
Sets the background color for the control.

#### Parameters


  -  *bSysColor* : int

    Indicates if the background color should be set to the system value. If this value is TRUE, cr is ignored.

  -  *cr=0* : int

    The requested background color. Used only if bSysColor is FALSE.

#### MFC References


  - CRichEditCtrl::SetEventMask

#### Return Value
The return value is the previous background color.

## [PyCRichEditCtrl](#pycricheditctrl).SetDefaultCharFormat

 __SetDefaultCharFormat( *charFormat* __ )
Sets the current default character formatting attributes in this[PyCRichEditCtrl](#pycricheditctrl)object.

#### Parameters


  -  *charFormat* : tuple

    A charformat tuple.  See __win32ui::CHARFORMAT tuple__ for details.

#### MFC References


  - CRichEditCtrl::SetDefaultCharFornmat

## [PyCRichEditCtrl](#pycricheditctrl).SetEventMask

int = __SetEventMask( *eventMask* __ )
Sets the event motification mask.

#### Parameters


  -  *eventMask* : int

    The new event mask.  Must be one of the win32con.ENM_* flags.

#### MFC References


  - CRichEditCtrl::SetEventMask

#### Return Value
The return value is the previous event mask.

## [PyCRichEditCtrl](#pycricheditctrl).SetModify

 __SetModify( *modified* __ )
Sets the modified flag for this control

#### Parameters


  -  *modified=1* : int

    Indicates the new value for the modified flag.

#### MFC References


  - CRichEditCtrl::SetModify

## [PyCRichEditCtrl](#pycricheditctrl).SetOptions

 __SetOptions( *op*  *, flags* __ )
Sets options for the control.

#### Parameters


  -  *op* : int

    Indicates the operation.  Must be one of the win32con.ECOOP_* flags.

  -  *flags* : int

    Indicates the options.  Must be one a combination of win32con.ECO_* flags.

#### MFC References


  - CRichEditCtrl::SetOptions

## [PyCRichEditCtrl](#pycricheditctrl).SetParaFormat

int = __SetParaFormat( *paraFormat* __ )
Sets the paragraph formatting

#### Parameters


  -  *paraFormat* : tuple

    A charformat tuple.  See __win32ui::PARAFORMAT tuple__ for details.

#### MFC References


  - CRichEditCtrl::SetParaFormat

#### Return Value
This function seems to return occasionally return failure, but 

the formatting is applied.  Therefore an exception is not raised on failure, 

but the BOOL return code is passed back.

## [PyCRichEditCtrl](#pycricheditctrl).SetReadOnly

 __SetReadOnly( *bReadOnly* __ )
Sets or clears the read-only status of the listbox.

#### Parameters


  -  *bReadOnly=1* : int

    The read-only state to set.

#### MFC References


  - CRichEditCtrl::SetReadOnly

## [PyCRichEditCtrl](#pycricheditctrl).SetSel

 __SetSel( *start*  *, end* __ )
Sets the selection in the edit control.

#### Parameters


  -  *start* : int

    Specifies the starting position. 

If start is 0 and end is -1, all the text in the edit control is selected. 

If start is -1, any current selection is removed.

  -  *end=start* : int

    Specifies the ending position.

#### Alternative Parameters


  -  *start,end)* 

    As for normal start, end args.

#### MFC References


  - CRichEditCtrl::SetSel

## [PyCRichEditCtrl](#pycricheditctrl).SetSelAndCharFormat

 __SetSelAndCharFormat( *charFormat* __ )
Sets the selection and char format.

#### Parameters


  -  *charFormat* : tuple

    A charformat tuple.  See __win32ui::CHARFORMAT tuple__ for details.

#### Comments
Highly optimised for speed for color editors.

#### MFC References


  - CRichEditCtrl::SetSelectionCharFormat

  - CRichEditCtrl::SetSel

## [PyCRichEditCtrl](#pycricheditctrl).SetSelectionCharFormat

 __SetSelectionCharFormat( *charFormat* __ )
Sets the current selections character formatting attributes.

#### Parameters


  -  *charFormat* : tuple

    A charformat tuple.  See __win32ui::CHARFORMAT tuple__ for details.

#### MFC References


  - CRichEditCtrl::SetSelectionCharFormat

## [PyCRichEditCtrl](#pycricheditctrl).SetTargetDevice

 __SetTargetDevice( *dc*  *, lineWidth* __ )
Sets the target device for the control

#### Parameters


  -  *dc* :[PyCDC](#pycdc)

    The new DC - may be None

  -  *lineWidth* : int

    Line width to use for formatting.

#### MFC References


  - CRichEditCtrl::SetTargetDevice

## [PyCRichEditCtrl](#pycricheditctrl).SetWordCharFormat

 __SetWordCharFormat( *charFormat* __ )
Sets the currently selected word's character formatting attributes.

#### Parameters


  -  *charFormat* : tuple

    A charformat tuple.  See __win32ui::CHARFORMAT tuple__ for details.

#### MFC References


  - CRichEditCtrl::SetWordCharFormat

## [PyCRichEditCtrl](#pycricheditctrl).StreamIn

(int,int) = __StreamIn( *format*  *, method* __ )
Invokes a callback to stream data into the control.

#### Parameters


  -  *format* : int

    The format.  One of the win32con.SF_* flags (SF_TEXT,SF_RTF)

  -  *method* : object

    A callable object (eg, a method or function) 

This method is called with a single integer param, which is the maximum number of 

bytes to fetch.  The method should return a zero length string, or None to 

finish the operation, and a string otherwise.

#### MFC References


  - CRichEditCtrl::StreamIn

#### Return Value
The return value is a tuple of (no bytes written, error code)

## [PyCRichEditCtrl](#pycricheditctrl).StreamOut

(int, int) = __StreamOut( *format*  *, method* __ )
Invokes a callback to stream data into the control.

#### Parameters


  -  *format* : int

    The format.  One of the win32con.SF_* flags (SF_TEXT,SF_RTF) and may also combine SFF_SELECTION.

  -  *method* : object

    A callable object (eg, a method or function) 

This method is called with a string parameter.  It should return an integer, zero to abort, non zero otherwise.

#### MFC References


  - CRichEditCtrl::StreamOut

#### Return Value
The return value is a tuple of (no bytes written, error code)