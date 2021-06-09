const artworks = require('./data.json');

exports.handler = async (event) => {
  const slug = event.path.replace('/api/artworks/', '');
  const artwork = artworks.find((m) => m.slug === slug);

  return {
    statusCode: 200,
    body: JSON.stringify(artwork),
  };
};
