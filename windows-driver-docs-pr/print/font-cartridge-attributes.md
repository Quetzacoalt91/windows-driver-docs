---
title: Font Cartridge Attributes
description: Font Cartridge Attributes
keywords:
- printer font descriptions WDK Unidrv , cartridges
- font cartridges WDK Unidrv
- cartridge fonts WDK Unidrv
ms.date: 01/27/2023
---

# Font Cartridge Attributes

[!include[Print Support Apps](../includes/print-support-apps.md)]

The following table contains attributes that can be included in a \*FontCartridge GPD entry.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Attribute Name</th>
<th>Attribute Parameter</th>
<th>Comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong><em>CartridgeName</strong></p></td>
<td><p>Text string representing the cartridge name.</p></td>
<td><p>Required, unless *<strong>rcCartridgeNameID</strong> is specified.</p></td>
</tr>
<tr class="even">
<td><p><strong></em>Fonts</strong></p></td>
<td><p>LIST of RC_UFM or RC_FONT resource identifiers representing fonts contained in the cartridge that are available for both portrait and landscape orientations.</p></td>
<td><p>At least one of <em><strong>Fonts</strong>,*<strong>PortraitFonts</strong> or *<strong>LandscapeFonts</strong> must be specified. Font resource identifiers should be numbered contiguously from 1.</p></td>
</tr>
<tr class="odd">
<td><p><strong></em>LandscapeFonts</strong></p></td>
<td><p>LIST of RC_UFM or RC_FONT resource identifiers representing fonts contained in the cartridge that are available only for landscape orientation.</p></td>
<td><p>At least one of <em><strong>Fonts</strong>,*<strong>PortraitFonts</strong> or *<strong>LandscapeFonts</strong> must be specified. Font resource identifiers should be numbered contiguously from 1.</p></td>
</tr>
<tr class="even">
<td><p><strong></em>PortraitFonts</strong></p></td>
<td><p>LIST of RC_UFM or RC_FONT resource identifiers representing fonts contained in the cartridge that are available only for portrait orientation.</p></td>
<td><p>At least one of <em><strong>Fonts</strong>,*<strong>PortraitFonts</strong> or *<strong>LandscapeFonts</strong> must be specified. Font resource identifiers should be numbered contiguously from 1.</p></td>
</tr>
<tr class="odd">
<td><p><strong></em>rcCartridgeNameID</strong></p></td>
<td><p>Resource identifier of a String resource representing the cartridge name.</p></td>
<td><p>Required, unless*<strong>CartridgeName</strong> is specified.</p></td>
</tr>
</tbody>
</table>
