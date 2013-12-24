---
layout: docs
title: Toolchain
permalink: /docs/toolchain/
---

The BitThunder toolchain, BTDK (BitThunder Development Kit) is now available
on Github.

## Quick Build Instructions

{% highlight bash %}
~ $ git clone git@github.com:bitthunder-toolchain/btdk.git
# Modify Makefile variables to suit.
~ $ make -j32
{% endhighlight %}

## Supported targets

BTDK currently supports the following targets:

    arm-eabi-bt         # The kernel mode compiler for ARM.
    arm-eabi-bitthunder # The user-mode compiler for ARM.

## Makefile variables.

    PREFIX - Default is /opt/btdk

## Using BTDK

To use the BTDK when building BitThunder, simply set the toolchain prefix
under the build-system configuration:

    make menuconfig

Under Build System set toolchain-prefix to:

    # For kernel mode applications:
	/opt/btdk/arm-eabi-bt-

	# For usermode applications:
	/opt/btdk/arm-eabi-bitthunder-


	