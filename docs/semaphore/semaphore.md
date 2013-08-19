---
layout: docs
title: Semaphores & Mutex's
next_section: usage-rules
permalink: /docs/api/semaphore/
header_path: os/include/process/bt_mutex.h
source_path: os/src/process/bt_mutex.c
---

Provides synchronisation objects between threads.
Later this API will allow named objects on the file-system, and for objects to be passed
between processes.

# Mutex API

The following table lists all functions related to the Mutex API.

<div class="mobile-side-scroller">
<table>
  <thead>
    <tr>
      <th>API</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>

	<tr>
      <td><p><code><a href="{{ site.url }}/api/process/bt_createprocess/">BT_CreateProcess()</a></code></p></td>
      <td><p>
		Creates a BitThunder process.
      </p></td>
    </tr>

	<tr>
      <td><p><code><a href="{{ site.url }}/api/process/bt_destroyprocess/">BT_DestroyProcess()</a></code></p></td>
      <td><p>
		Destroys a BitThunder process.
      </p></td>
    </tr>

	<tr>
      <td><p><code><a href="{{ site.url }}/api/process/bt_getprocesshandle/">BT_GetProcessHandle()</a></code></p></td>
      <td><p>
		Gets the handle of the current process.
      </p></td>
    </tr>

  </tbody>
</table>
</div>

# Semaphore API

Currently the semaphore API has not been exposed.

# Kernel-space / Driver API

# Design Overview
These APIs are simply wrappers to the underlying tasking kernel used, usually FreeRTOS.
However direct implementations may be provided when using the BtKernel when available.

# Further Reading

The full API is defined under:

{% include api/header-path.md %}

See the implementation under:

{% include api/source-path.md %}
