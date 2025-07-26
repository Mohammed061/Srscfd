{% schema %}
{
  "name": "Pyramida Tekst Sectie",
  "settings": [
    {
      "type": "text",
      "id": "titel",
      "label": "Titel",
      "default": "Pyramida Wellness Clinic"
    },
    {
      "type": "textarea",
      "id": "beschrijving",
      "label": "Beschrijving",
      "default": "Ervaar de magie van oud-Egyptische healing."
    },
    {
      "type": "color",
      "id": "achtergrondkleur",
      "label": "Achtergrondkleur",
      "default": "#f4f0e2"
    },
    {
      "type": "color",
      "id": "tekstkleur",
      "label": "Tekstkleur",
      "default": "#000000"
    }
  ],
  "presets": [
    {
      "name": "Pyramida Tekst Sectie",
      "category": "Inhoud"
    }
  ]
}
{% endschema %}

<div style="padding: 40px; background: {{ section.settings.achtergrondkleur }}; text-align: center; color: {{ section.settings.tekstkleur }};">
  <h2>{{ section.settings.titel }}</h2>
  <p>{{ section.settings.beschrijving }}</p>
</div>
