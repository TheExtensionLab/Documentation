---
layout: page
title: Developer Information
date: 2015-01-18 16:50:00
category: status-colors
order: 4
---

A few key Overview details:

**Modman:** Yes

**Composer:** Yes

**GitHub:** https://github.com/TheExtensionLab/StatusColors

**Core Hacks:** 0

**Class Rewrites:** 0

We are also providing you with the config.xml, consider this the "Amazon Look Inside" for extensions for a sneak preview into what the extension does and how it does it. (e.g does it use rewrites? **(the answer is NO)**)

```
<?xml version="1.0"?>
<config>
    <modules>
        <TheExtensionLab_StatusColors>
            <version>0.1.0</version>
        </TheExtensionLab_StatusColors>
    </modules>

    <global>
        <blocks>
            <theextensionlab_statuscolors>
                <class>TheExtensionLab_StatusColors_Block</class>
            </theextensionlab_statuscolors>
        </blocks>
        <helpers>
            <theextensionlab_statuscolors>
                <class>TheExtensionLab_StatusColors_Helper</class>
            </theextensionlab_statuscolors>
        </helpers>
        <models>
            <theextensionlab_statuscolors>
                <class>TheExtensionLab_StatusColors_Model</class>
                <resourceModel>theextensionlab_statuscolors_resource</resourceModel>
            </theextensionlab_statuscolors>
            <theextensionlab_statuscolors_resource>
                <class>TheExtensionLab_StatusColors_Model_Resource</class>
            </theextensionlab_statuscolors_resource>
        </models>
        <resources>
            <theextensionlab_statuscolors_setup>
                <setup>
                    <module>TheExtensionLab_StatusColors</module>
                    <class>TheExtensionLab_StatusColors_Model_Resource_Setup</class>
                </setup>
            </theextensionlab_statuscolors_setup>
        </resources>
    </global>

    <adminhtml>
        <layout>
            <updates>
                <theextensionlab_statuscolors>
                    <file>theextensionlab/statuscolors.xml</file>
                </theextensionlab_statuscolors>
            </updates>
        </layout>
        <events>
            <adminhtml_block_html_before>
                <observers>
                    <theextensionlab_statuscolors>
                        <class>TheExtensionLab_StatusColors_Model_Observer</class>
                        <method>adminhtmlBlockHtmlBefore</method>
                    </theextensionlab_statuscolors>
                </observers>
            </adminhtml_block_html_before>
            <core_block_abstract_to_html_after>
                <observers>
                    <theextensionlab_statuscolors>
                        <class>TheExtensionLab_StatusColors_Model_Observer</class>
                        <method>coreBlockAbstractToHtmlAfter</method>
                    </theextensionlab_statuscolors>
                </observers>
            </core_block_abstract_to_html_after>
            <controller_action_predispatch_adminhtml_system_config_edit>
                <observers>
                    <theextensionlab_statuscolors>
                        <class>TheExtensionLab_StatusColors_Model_Observer</class>
                        <method>controllerActionPredispatchAdminhtmlSystemConfigEdit</method>
                    </theextensionlab_statuscolors>
                </observers>
            </controller_action_predispatch_adminhtml_system_config_edit>
        </events>
    </adminhtml>
</config>
```
