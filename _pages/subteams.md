---
layout: page
title: Subteams
permalink: /subteams/
---

A key part of the HTA ESIG are the various subteams where members discuss and collaborate on more specialized topics. 

Are you interested in joining one of the sub-teams? Either reach out to the lead directly or send an email to <a href="mailto:htasig@psiweb.org">htasig@psiweb.org</a> and we will put you in touch with the lead.

Please note, you must first be a member of the HTA ESIG to join one of the sub-teams.

## Subteams (incomplete)
<table>
    <thead>
        <tr>
            <th>Subteam</th>
            <th>Related to <a href="/about">objective</a> </th>
            <th>Lead</th>
            <th>Members</th>
            <th>Details</th>
            <th>Active?</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.subteams %}
        <tr>
            <td>{{ item.name }}</td>
            <td>{{ item.sig_objective }}</td>
            <td>{{ item.lead }}</td>
            <td>{{ item.members }}</td>
            <td>{{ item.details }}</td>
            <td>{{ item.active }}</td>
        </tr>
        {% endfor %}
    </tbody>
</table>
