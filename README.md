/The following Script for the Response Validation is written by Javascript and was Tested using Cypress/
it('Api Respone', () => {
cy.request('http://localhost:8080/');

/Let the displayed Text of GET/:INPUT has a class called body/
cy.get('.body').should('contain', 'Get/:input').and('response.status', '200')


})
